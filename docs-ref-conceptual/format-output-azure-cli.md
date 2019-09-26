---
title: Formats de sortie pour Azure CLI
description: Apprenez à mettre la sortie des commandes Azure CLI aux formats de listes, de tableaux ou de json.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/23/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 125055eec956e56c95af9a1c24ee4254e77556e6
ms.sourcegitcommit: 5b9b4446c08b94256ced7f63c145b493ba8b50df
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2019
ms.locfileid: "71217452"
---
# <a name="output-formats-for-azure-cli-commands"></a>Formats de sortie pour les commandes Azure CLI

Azure CLI utilise JSON comme format de sortie par défaut, mais il propose d’autres formats.  Utilisez le paramètre `--output` (`--out` ou `-o`) pour formater la sortie de l’interface CLI. Les valeurs d’argument et les types de sortie sont :

--output | Description
---------|-------------------------------
`json`   | Chaîne JSON. Il s’agit du paramètre par défaut.
`jsonc`  | JSON coloré.
`yaml`   | YAML, une alternative à JSON pouvant être lue par la machine.
`table`  | Table ASCII avec des clés en tant qu’en-têtes de colonne.
`tsv`    | Valeurs séparées par des tabulations, sans clés

## <a name="json-output-format"></a>Format de sortie JSON

L’exemple suivant affiche la liste des machines virtuelles de vos abonnements au format JSON par défaut.

```azurecli-interactive
az vm list --output json
```

Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="yaml-output-format"></a>Format de sortie YAML

Le format `yaml` affiche la sortie en tant que [YAML](http://yaml.org/), un format de sérialisation de données en texte brut. YAML est souvent plus simple à lire que JSON et se mappe facilement vers ce format. Certaines applications et commandes CLI utilisent YAML en tant qu’entrée de configuration, plutôt que JSON.

```azurecli-interactive
az vm list --out yaml
```

Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a>Format de sortie de la table

Le format `table` imprime la sortie sous forme de tableau ASCII, ce qui la rend facile à lire et à analyser. Les objets imbriqués ne sont pas inclus dans le tableau de sortie, mais peuvent toujours être filtrés dans le cadre d’une requête. Certains champs ne sont pas compris dans le tableau. Ainsi, ce format est le plus approprié si vous souhaitez obtenir un aperçu des données rapide et consultable pour un être humain.

```azurecli-interactive
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée. L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.

```azurecli-interactive
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> Certaines clés ne sont pas imprimées dans l’affichage du tableau par défaut. Il s’agit de `id`, `type`, et `etag`. Si vous avez besoin de les voir dans votre sortie, vous pouvez utiliser la fonction JMESPath de régénération des clés pour modifier le nom de clé et éviter le filtrage.
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

Pour plus d’informations concernant l’utilisation des requêtes pour filtrer les données, consultez [Utiliser des requêtes JMESPath avec Azure CLI](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>Format de sortie TSV

Le format de sortie `tsv` retourne des valeurs séparées par des tabulations et des sauts de ligne sans mise en forme, clés ou autres symboles supplémentaires. Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée. Comme pour le format `table`, le format `tsv` n’imprime pas les objets imbriqués.

L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

L’une des restrictions du format de sortie TSV est qu’il n’existe aucune garantie quant à l’ordre de la sortie. L’interface CLI fait de son mieux pour préserver l’ordre en triant les clés dans le code JSON de la réponse par ordre alphabétique, puis en imprimant leurs valeurs dans l’ordre pour la sortie TSV. Il n’est donc pas garanti que l’ordre soit toujours le même puisque le format de la réponse du service Azure peut changer.

Pour appliquer un ordre cohérent, vous devez utiliser le paramètre `--query` et le format de [liste à sélection multiple](query-azure-cli.md#get-multiple-values). Quand une commande CLI retourne un dictionnaire JSON unique, utilisez le format général `[key1, key2, ..., keyN]` pour forcer l’ordre des clés.  Pour les commandes CLI qui retournent un tableau, utilisez le format général `[].[key1, key2, ..., keyN]` pour ordonner les valeurs de colonne.

Par exemple, pour ordonner les informations affichées ci-dessus par ID, emplacement, groupe de ressources et nom de machine virtuelle :

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

L’exemple suivant montre comment la sortie `tsv` peut être transmise à d’autres commandes dans Bash. La requête permet de filtrer la sortie et de forcer l’ordre, `grep` sélectionne les éléments contenant le texte « RGD », puis la commande `cut` sélectionne le quatrième champ pour afficher le nom de la machine virtuelle dans la sortie.

```bash
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a>Définir le format de sortie par défaut

Utilisez la commande interactive `az configure` pour configurer votre environnement et établir des paramètres par défaut pour les formats de sortie. Le format de sortie par défaut est `json`.

```azurecli-interactive
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

Pour en savoir plus sur la configuration de votre environnement, consultez [Configuration d’Azure CLI](/cli/azure/azure-cli-configuration).
