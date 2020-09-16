---
title: Utiliser Azure CLI efficacement
description: Conseils pour utiliser Azure CLI efficacement
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 53fa51e3d17069c9d3af62d53214d366f33779b4
ms.sourcegitcommit: 6c3032b1d74c65a8f186b3063ab6b301350e3704
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2020
ms.locfileid: "90012729"
---
# <a name="use-azure-cli-effectively"></a>Utiliser Azure CLI efficacement

Par souci de clarté, les scripts Bash sont utilisés inline. Les exemples PowerShell ou de commandes Windows sont listés dans l’annexe, que vous pouvez utiliser pour générer des exemples similaires.

## <a name="output-formatting-json-table-or-tsv"></a>Mise en forme de la sortie (json, table ou tsv)

1. `json` est le format par défaut de l’interface CLI, conçu pour vous fournir les informations les plus complètes. Si vous préférez un format différent, utilisez l’argument `--output` pour remplacer un appel de commande individuel, ou `az configure` pour mettre à jour votre configuration globale par défaut. Notez que le format JSON conserve les guillemets doubles, ce qui le rend généralement inadapté aux scripts.

2. Le format `table` est utile pour obtenir un résumé des informations ciblées, en particulier pour les commandes de liste. Si vous n’aimez pas les champs dans le format de table par défaut (ou qu’il n’existe pas de format par défaut), vous pouvez utiliser `--output json` pour afficher toutes les informations ou tirer parti de `--query` pour spécifier le format de votre choix.

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. Le format `tsv` est utile à des fins de sorties et de scripts concis. Le format tsv supprimera les guillemets doubles que le format JSON conserve. Pour spécifier le format souhaité pour TSV, utilisez l’argument `--query`.

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a>Transmettre des valeurs d’une commande à une autre

1. Si la valeur est utilisée plusieurs fois, affectez-la à une variable. Notez l’utilisation de `-o tsv` dans l’exemple suivant :

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. Si la valeur n’est utilisée qu’une seule fois, envisagez une canalisation :
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. Pour les listes, tenez compte des suggestions suivantes :

   Si vous avez besoin de davantage de contrôle sur le résultat, utilisez la boucle « for » :
    ```sh
    #!/usr/bin/env bash
    for vm in $(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv); do
        echo stopping $vm
        az vm stop --ids $vm
        if [ $? -ne 0 ]; then
            echo "Failed to stop $vm"
            exit 1
        fi
        echo $vm stopped
    done
    ```

    Vous pouvez également utiliser `xargs` et envisager d’utiliser l’indicateur `-P` pour exécuter les opérations en parallèle afin d’améliorer les performances :
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    Enfin, Azure CLI propose une prise en charge intégrée pour traiter les commandes avec plusieurs `--ids` en parallèle afin d’obtenir le même effet que xargs. Notez que `@-` est utilisé pour récupérer des valeurs à partir du canal :
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a>Opérations asynchrones

Un grand nombre de commandes et groupes exposent des indicateurs `--no-wait` sur leurs opérations de longue durée ainsi qu’une commande `wait` dédiée. Ils deviennent pratiques dans certains scénarios :

1. Nettoyage des ressources quand vous ne vous fiez pas au nettoyage pour une opération ultérieure, telle que la suppression d’un groupe de ressources :
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. Lorsque vous souhaitez créer plusieurs ressources indépendantes en parallèle. Cela est similaire à la création et à la jointure de threads :

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a>Arguments de mise à jour génériques

La plupart des commandes de mise à jour dans l’interface CLI disposent des trois arguments génériques suivants : `--add`, `--set` et `--remove`. Ces arguments sont puissants, mais souvent moins pratiques que les arguments fortement typés généralement proposés dans les commandes de mise à jour. L’interface CLI fournit des arguments fortement typés pour la plupart des scénarios courants en vue d’une plus grande facilité d’utilisation mais, si la propriété que vous souhaitez définir n’est pas listée, les arguments de mise à jour génériques vous indiquent souvent une voie à suivre pour vous débloquer sans avoir à attendre une nouvelle version.

1. Comme la syntaxe de mise à jour générique n’est pas la plus conviviale, vous devez faire preuve de patience.
2. Vérifiez si le groupe `Generic Update Arguments` est exposé dans la commande de mise à jour. Si ce n’est pas le cas, vous devez signaler un problème. Si c’est le cas, vous pouvez essayer de l’utiliser.
3. Utilisez la commande `show` sur la ressource qui vous intéresse pour déterminer le chemin à fournir dans les arguments génériques. Par exemple, avant d’essayer `az vm update`, exécutez `az vm show` pour identifier le chemin correct. En règle générale, vous allez utiliser la syntaxe à point pour accéder aux propriétés du dictionnaire et les crochets pour indexer dans des listes.
4. Consultez des exemples fonctionnels pour commencer. `az vm update -h` en contient d’excellents.
5. `--set` et `--add` prennent une liste de paires clé-valeur au format `<key1>=<value1> <key2>=<value2>`. Utilisez-les pour construire des charges utiles complexes. Si la syntaxe a trop de messages, envisagez d’utiliser une chaîne JSON. Par exemple, pour attacher un nouveau disque de données à une machine virtuelle :
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. Il peut s’avérer plus utile de tirer parti de la convention `@{file}` de l’interface CLI, en plaçant le JSON dans un fichier et en le chargeant. Cela simplifie la commande ci-dessus en :
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a>Commandes de ressources génériques - `az resource`

Il peut arriver qu’un service qui vous intéresse n’ait pas de couverture de commande d’interface CLI. Vous pouvez employer les commandes `az resource create/show/list/delete/update/invoke-action` pour utiliser ces ressources. Voici quelques suggestions :
1. Si seules les commandes `create/update` sont impliquées, envisagez d’utiliser `az group deployment create`. Mettez à profit les [modèles de démarrage rapide Microsoft Azure](https://github.com/Azure/azure-quickstart-templates) pour obtenir des exemples fonctionnels.
2. Consultez les informations de référence sur l’API REST pour la charge utile de demande, l’URL et la version de l’API. À titre d’exemple, consultez les commentaires de la communauté sur [la façon de créer des ressources Application Insights](https://github.com/Azure/azure-cli/issues/5543).

## <a name="rest-api-command---az-rest"></a>Commande API REST - `az rest`

Si aucun argument de mise à jour générique ni `az resource` ne répond à vos besoins, vous pouvez utiliser la commande `az rest` pour appeler l’API REST. Elle s’authentifie automatiquement à l’aide des informations d’identification de connexion et définit l’en-tête `Content-Type: application/json`.

Cela est très utile pour appeler l’[API Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) qui n’est pas prise en charge pour l’instant par les commandes d’interface CLI ([n°12946](https://github.com/Azure/azure-cli/issues/12946)).

Par exemple, pour mettre à jour `redirectUris` pour une [application](/graph/api/resources/application?view=graph-rest-1.0), nous appelons l’API REST [Mettre à jour l’application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) avec :

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

Lorsque vous utilisez `--uri-parameters` pour les demandes sous la forme d’OData, veillez à placer `$` dans une séquence d’échappement dans différents environnements : dans `Bash`, placez `$` dans la séquence d’échappement `\$` et dans `PowerShell`, placez `$` dans la séquence `` `$``

## <a name="quoting-issues"></a>Problèmes liés aux guillemets

Cela devient un problème car, lorsque l’interface de commande (Bash, Zsh, invite de commandes Windows, PowerShell, etc.) analyse la commande CLI, elle interprète les guillemets et les espaces. Reportez-vous toujours aux documents lorsque vous hésitez quant à l’utilisation d’un interpréteur de commandes :

- Bash : [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)
- PowerShell : [À propos des règles liées aux guillemets](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)
    - En raison d’un problème connu ([n°1995](https://github.com/PowerShell/PowerShell/issues/1995)) de PowerShell, certaines règles d’échappement supplémentaires s’appliquent. Pour plus d’informations, consultez [Problèmes liés aux guillemets avec PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).
- Invite de commandes Windows : [Guide pratique pour placer dans une séquence d’échappement des caractères, délimiteurs et guillemets au niveau de la ligne de commande Windows](https://ss64.com/nt/syntax-esc.html)

Pour éviter des résultats imprévus, voici quelques suggestions :

1. Si la valeur contient un espace blanc, vous devez la wrapper entre guillemets.
2. Dans Bash ou Windows PowerShell, les guillemets simples et doubles sont interprétés tandis que dans l’invite de commandes Windows, seuls les guillemets doubles sont gérés, ce qui signifie que les guillemets simples sont interprétés comme une partie de la valeur.
3. Si votre commande s’exécute uniquement sur Bash (ou Zsh), l’utilisation de guillemets simples présente l’avantage de conserver le contenu à l’intérieur. Cela peut être très utile lors de la fourniture de JSON inline. Par exemple, la commande suivante fonctionne dans Bash : `'{"foo": "bar"}'`
4. Si votre commande s’exécute sur l’invite de commandes Windows, vous devez utiliser exclusivement des guillemets doubles. Si la valeur contient des guillemets doubles, vous devez la placer dans une séquence d’échappement : `"i like to use \" a lot"`. L’équivalent pour l’invite de commandes de la commande ci-dessus est : `"{\"foo\": \"bar\"}"`
5. Les variables exportées dans Bash entre guillemets doubles sont évaluées. Si ce n’est pas ce que vous voulez, utilisez de nouveau `\ ` pour placer la valeur dans une séquence d’échappement comme `"\$var"` ou utilisez des guillemets simples `'$var'`.
6. Quelques arguments CLI, dont les arguments de mise à jour génériques, prennent une liste de valeurs séparées par des espaces, comme `<key1>=<value1> <key2>=<value2>`. Étant donné que le nom de la clé et la valeur peuvent accepter une chaîne arbitraire susceptible de contenir un espace blanc, l’utilisation de guillemets est nécessaire. Wrappez la paire, et non la clé ou la valeur individuelle. `"my name"=john` est donc incorrect. Utilisez plutôt `"my name=john"`. Par exemple :
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. Utilisez la convention `@<file>` de l’interface CLI pour le chargement à partir d’un fichier afin de contourner les mécanismes d’interprétation de l’interpréteur de commandes :
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. Lorsqu’un argument CLI indique qu’il accepte une liste de valeurs séparées par des espaces, les formats acceptés sont les suivants :
    - `--arg foo bar`: OK. Liste de valeurs séparées par des espaces, sans guillemets
    - `--arg "foo" "bar"`: OK : Liste de valeurs séparées par des espaces, avec guillemets
    - `--arg "foo bar"`: BAD. Il s’agit d’une chaîne contenant un espace et non d’une liste de valeurs séparées par des espaces.
9. Lors de l’exécution de commandes Azure CLI dans PowerShell, l’analyse des erreurs se produit quand les arguments contiennent des caractères spéciaux de PowerShell, comme `@`. Vous pouvez résoudre ce problème en ajoutant `` ` `` avant le caractère spécial pour le placer dans une séquence d’échappement, ou en mettant l’argument entre guillemets simples ou doubles `'`/`"`. Par exemple, `az group deployment create --parameters @parameters.json` ne fonctionne pas dans PowerShell, car `@` est analysé en tant que [symbole de projection](/powershell/module/microsoft.powershell.core/about/about_splatting). Pour résoudre ce problème, vous pouvez remplacer l’argument par `` `@parameters.json`` ou `'@parameters.json'`.
10. Lorsque vous utilisez `--query` avec une commande, certains caractères de [JMESPath](https://jmespath.org/specification.html) doivent être placés dans une séquence d’échappement dans l’interpréteur de commandes. Par exemple, dans Bash :
    ```sh
    # Wrong, as the dash needs to be quoted in a JMESPath query
    $ az version --query azure-cli
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Wrong, as the dash needs to be quoted in a JMESPath query, but quotes are interpreted by Bash
    $ az version --query "azure-cli"
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Correct
    $ az version --query '"azure-cli"'
    "2.5.1"

    $ az version --query \"azure-cli\"
    "2.5.1"

    $ az version --query "\"azure-cli\""
    "2.5.1"
    ```

    Dans l’invite de commandes :
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    Dans PowerShell (des séquences d’échappement supplémentaires sont nécessaires) :
    ```powershell
    > az version --query '\"azure-cli\"'
    "2.5.1"

    > az version --query "\`"azure-cli\`""
    "2.5.1"

    > az version --query "\""azure-cli\"""
    "2.5.1"

    > az --% version --query "\"azure-cli\""
    "2.5.1"

    > az --% version --query \"azure-cli\"
    "2.5.1"
    ```

11. La meilleure façon de résoudre un problème lié aux guillemets consiste à exécuter la commande avec l’indicateur `--debug`. Il révèle les arguments réels reçus par l’interface CLI dans la [syntaxe de Python](https://docs.python.org/3/tutorial/introduction.html#strings). Par exemple, dans Bash :

    ```sh
    # Wrong, as quotes and spaces are interpreted by Bash
    $ az {"key": "value"} --debug
    Command arguments: ['{key:', 'value}', '--debug']

    # Wrong, as quotes are interpreted by Bash
    $ az {"key":"value"} --debug
    Command arguments: ['{key:value}', '--debug']

    # Correct
    $ az '{"key":"value"}' --debug
    Command arguments: ['{"key":"value"}', '--debug']

    # Correct
    $ az "{\"key\":\"value\"}" --debug
    Command arguments: ['{"key":"value"}', '--debug']
    ```

## <a name="work-behind-a-proxy"></a>Travail derrière un proxy

Le proxy est courant derrière le réseau d’entreprise ou introduit par des outils de suivi tels que Fiddler, mitmproxy, etc. Si le proxy utilise des certificats auto-signés, la bibliothèque de [demandes](https://github.com/kennethreitz/requests) de Python que l’interface CLI utilise va générer `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`. Il existe 2 moyens de gérer cette erreur :

1. Définissez la variable d’environnement `REQUESTS_CA_BUNDLE` sur le chemin du fichier du certificat de groupement d’autorités de certification au format PEM. Cette option est recommandée si vous utilisez l’interface CLI fréquemment derrière un proxy d’entreprise. Le groupement d’autorités de certification par défaut utilisé par l’interface CLI se trouve sur `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` sur Windows et ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` sur Linux. Vous pouvez ajouter le certificat du serveur proxy à ce fichier ou copier le contenu dans un autre fichier de certificat, puis définir `REQUESTS_CA_BUNDLE` sur celui-ci. Par exemple :

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   Il est fréquemment demandé si les variables d’environnement `HTTP_PROXY` ou `HTTPS_PROXY` doivent ou non être définies, et la réponse est que cela dépend. Pour Fiddler sur Windows, la variable agit par défaut en tant que proxy système au démarrage et vous n’avez pas besoin de définir quoi que ce soit. Si l’option est désactivée ou que vous utilisez d’autres outils qui ne fonctionnent pas en tant que proxy système, vous devez les définir. Comme presque tout le trafic de l’interface CLI est basé sur SSL, seule `HTTPS_PROXY` doit être définie. Si vous ne savez pas, il vous suffit de les définir, mais n’oubliez pas d’annuler cette configuration après l’arrêt du proxy. Pour Fiddler, la valeur par défaut est `http://localhost:8888`.

   Pour plus d’informations, consultez le [blog de Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).

2. Désactivez la vérification du certificat sur Azure CLI en définissant la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`. Cette solution n’est pas sûre, mais elle est valable pendant une brève période comme la capture d’une trace réseau pour une commande spécifique. Il convient de désactiver cette option rapidement une fois l’opération terminée. Cela peut ne pas fonctionner pour certaines commandes de plan de données en raison des limitations du SDK sous-jacent.

## <a name="concurrent-builds"></a>Builds simultanées

Si vous utilisez az sur un ordinateur de build et que plusieurs travaux peuvent être exécutés en parallèle, il existe un risque que les jetons de connexion soient partagés entre deux travaux de build si les travaux sont exécutés sous le même nom d’utilisateur du système d’exploitation.  Pour éviter une telle confusion, définissez AZURE_CONFIG_DIR sur un répertoire dans lequel les jetons de connexion doivent être stockés.  Il peut s’agir d’un dossier créé de manière aléatoire, ou simplement du nom de l’espace de travail Jenkins, comme suit : ```AZURE_CONFIG_DIR=.```

## <a name="appendix"></a>Annexe

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a>Scripts de commandes par lot Windows pour l’enregistrement dans des variables et une utilisation ultérieure

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a>Scripts Windows PowerShell pour l’enregistrement dans des variables et une utilisation ultérieure

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a>Scripts de commandes par lot Windows pour parcourir une liste
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a>Scripts Windows PowerShell pour parcourir une liste
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a>Variables d’environnement CLI

|  Variable d’environnement          | Description            |
|--------------------------------|------------------------|
| **AZURE_CONFIG_DIR**           | Répertoire de configuration globale pour les fichiers de configuration, les journaux et la télémétrie. Si elle n’est pas spécifiée, la valeur par défaut est `~/.azure`. |
| **AZURE_EXTENSION_DIR**        | Répertoire d’installation des extensions. Si elle n’est pas spécifiée, la valeur par défaut est le répertoire `cliextensions` dans le répertoire de configuration globale. |
