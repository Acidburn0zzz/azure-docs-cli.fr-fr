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
# <a name="use-azure-cli-effectively"></a><span data-ttu-id="6a45d-103">Utiliser Azure CLI efficacement</span><span class="sxs-lookup"><span data-stu-id="6a45d-103">Use Azure CLI effectively</span></span>

<span data-ttu-id="6a45d-104">Par souci de clarté, les scripts Bash sont utilisés inline.</span><span class="sxs-lookup"><span data-stu-id="6a45d-104">For clarity, Bash scripts are used inline.</span></span> <span data-ttu-id="6a45d-105">Les exemples PowerShell ou de commandes Windows sont listés dans l’annexe, que vous pouvez utiliser pour générer des exemples similaires.</span><span class="sxs-lookup"><span data-stu-id="6a45d-105">Windows batch or PowerShell examples are listed in the appendix, which you can use to build similar examples.</span></span>

## <a name="output-formatting-json-table-or-tsv"></a><span data-ttu-id="6a45d-106">Mise en forme de la sortie (json, table ou tsv)</span><span class="sxs-lookup"><span data-stu-id="6a45d-106">Output formatting (json, table, or tsv)</span></span>

1. <span data-ttu-id="6a45d-107">`json` est le format par défaut de l’interface CLI, conçu pour vous fournir les informations les plus complètes.</span><span class="sxs-lookup"><span data-stu-id="6a45d-107">`json` format is the CLI's default, and is intended to give you the most comprehensive information.</span></span> <span data-ttu-id="6a45d-108">Si vous préférez un format différent, utilisez l’argument `--output` pour remplacer un appel de commande individuel, ou `az configure` pour mettre à jour votre configuration globale par défaut.</span><span class="sxs-lookup"><span data-stu-id="6a45d-108">If you prefer a different format, use the `--output` argument to override for an individual command invocation, or use `az configure` to update your global default.</span></span> <span data-ttu-id="6a45d-109">Notez que le format JSON conserve les guillemets doubles, ce qui le rend généralement inadapté aux scripts.</span><span class="sxs-lookup"><span data-stu-id="6a45d-109">Note that JSON format preserves the double quotes, generally making in unsuitable for scripting purposes.</span></span>

2. <span data-ttu-id="6a45d-110">Le format `table` est utile pour obtenir un résumé des informations ciblées, en particulier pour les commandes de liste.</span><span class="sxs-lookup"><span data-stu-id="6a45d-110">`table` is useful for getting a summary of focused information, particularly for list commands.</span></span> <span data-ttu-id="6a45d-111">Si vous n’aimez pas les champs dans le format de table par défaut (ou qu’il n’existe pas de format par défaut), vous pouvez utiliser `--output json` pour afficher toutes les informations ou tirer parti de `--query` pour spécifier le format de votre choix.</span><span class="sxs-lookup"><span data-stu-id="6a45d-111">If you do not like the fields in the default table format (or there isn't a default format), you can use `--output json` to see all information, or leverage `--query` to specify a format you like.</span></span>

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. <span data-ttu-id="6a45d-112">Le format `tsv` est utile à des fins de sorties et de scripts concis.</span><span class="sxs-lookup"><span data-stu-id="6a45d-112">`tsv` is useful for concise output and scripting purposes.</span></span> <span data-ttu-id="6a45d-113">Le format tsv supprimera les guillemets doubles que le format JSON conserve.</span><span class="sxs-lookup"><span data-stu-id="6a45d-113">The tsv will strip double quotes that the JSON format preserves.</span></span> <span data-ttu-id="6a45d-114">Pour spécifier le format souhaité pour TSV, utilisez l’argument `--query`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-114">To specify the format you want for TSV, use the `--query` argument.</span></span>

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a><span data-ttu-id="6a45d-115">Transmettre des valeurs d’une commande à une autre</span><span class="sxs-lookup"><span data-stu-id="6a45d-115">Pass values from one command to another</span></span>

1. <span data-ttu-id="6a45d-116">Si la valeur est utilisée plusieurs fois, affectez-la à une variable.</span><span class="sxs-lookup"><span data-stu-id="6a45d-116">If the value will be used more than once, assign it to a variable.</span></span> <span data-ttu-id="6a45d-117">Notez l’utilisation de `-o tsv` dans l’exemple suivant :</span><span class="sxs-lookup"><span data-stu-id="6a45d-117">Note the use of `-o tsv` in the following example:</span></span>

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. <span data-ttu-id="6a45d-118">Si la valeur n’est utilisée qu’une seule fois, envisagez une canalisation :</span><span class="sxs-lookup"><span data-stu-id="6a45d-118">If the value is used only once, consider piping:</span></span>
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. <span data-ttu-id="6a45d-119">Pour les listes, tenez compte des suggestions suivantes :</span><span class="sxs-lookup"><span data-stu-id="6a45d-119">For lists consider the following suggestions:</span></span>

   <span data-ttu-id="6a45d-120">Si vous avez besoin de davantage de contrôle sur le résultat, utilisez la boucle « for » :</span><span class="sxs-lookup"><span data-stu-id="6a45d-120">If you need more controls on the result, use "for" loop:</span></span>
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

    <span data-ttu-id="6a45d-121">Vous pouvez également utiliser `xargs` et envisager d’utiliser l’indicateur `-P` pour exécuter les opérations en parallèle afin d’améliorer les performances :</span><span class="sxs-lookup"><span data-stu-id="6a45d-121">Alternatively, use `xargs` and consider using the `-P` flag to run the operations in parallel for improved performance:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    <span data-ttu-id="6a45d-122">Enfin, Azure CLI propose une prise en charge intégrée pour traiter les commandes avec plusieurs `--ids` en parallèle afin d’obtenir le même effet que xargs.</span><span class="sxs-lookup"><span data-stu-id="6a45d-122">Finally, Azure CLI has built-in support to process commands with multiple `--ids` in parallel to achieve the same effect of xargs.</span></span> <span data-ttu-id="6a45d-123">Notez que `@-` est utilisé pour récupérer des valeurs à partir du canal :</span><span class="sxs-lookup"><span data-stu-id="6a45d-123">Note that `@-` is used to get values from the pipe:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a><span data-ttu-id="6a45d-124">Opérations asynchrones</span><span class="sxs-lookup"><span data-stu-id="6a45d-124">Async operations</span></span>

<span data-ttu-id="6a45d-125">Un grand nombre de commandes et groupes exposent des indicateurs `--no-wait` sur leurs opérations de longue durée ainsi qu’une commande `wait` dédiée.</span><span class="sxs-lookup"><span data-stu-id="6a45d-125">Many commands and group expose `--no-wait` flags on their long-running operations as well as a dedicated `wait` command.</span></span> <span data-ttu-id="6a45d-126">Ils deviennent pratiques dans certains scénarios :</span><span class="sxs-lookup"><span data-stu-id="6a45d-126">These become handy for certain scenarios:</span></span>

1. <span data-ttu-id="6a45d-127">Nettoyage des ressources quand vous ne vous fiez pas au nettoyage pour une opération ultérieure, telle que la suppression d’un groupe de ressources :</span><span class="sxs-lookup"><span data-stu-id="6a45d-127">Cleaning up resources when you aren't relying on the clean up for some subsequent operation, such as deleting a resource group:</span></span>
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. <span data-ttu-id="6a45d-128">Lorsque vous souhaitez créer plusieurs ressources indépendantes en parallèle.</span><span class="sxs-lookup"><span data-stu-id="6a45d-128">When you want to create multiple independent resources in parallel.</span></span> <span data-ttu-id="6a45d-129">Cela est similaire à la création et à la jointure de threads :</span><span class="sxs-lookup"><span data-stu-id="6a45d-129">This is similar to creating and joining threads:</span></span>

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a><span data-ttu-id="6a45d-130">Arguments de mise à jour génériques</span><span class="sxs-lookup"><span data-stu-id="6a45d-130">Generic update arguments</span></span>

<span data-ttu-id="6a45d-131">La plupart des commandes de mise à jour dans l’interface CLI disposent des trois arguments génériques suivants : `--add`, `--set` et `--remove`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-131">Most update commands in the CLI feature the three generic arguments: `--add`, `--set` and `--remove`.</span></span> <span data-ttu-id="6a45d-132">Ces arguments sont puissants, mais souvent moins pratiques que les arguments fortement typés généralement proposés dans les commandes de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="6a45d-132">These arguments are powerful but often less convenient than the strongly-typed arguments typically featured in update commands.</span></span> <span data-ttu-id="6a45d-133">L’interface CLI fournit des arguments fortement typés pour la plupart des scénarios courants en vue d’une plus grande facilité d’utilisation mais, si la propriété que vous souhaitez définir n’est pas listée, les arguments de mise à jour génériques vous indiquent souvent une voie à suivre pour vous débloquer sans avoir à attendre une nouvelle version.</span><span class="sxs-lookup"><span data-stu-id="6a45d-133">The CLI provides strongly-typed arguments for most common scenarios for ease-of-use, but if the property you want to set isn't listed, the generic update arguments will often present a path forward to unblock you without having to wait for a new release.</span></span>

1. <span data-ttu-id="6a45d-134">Comme la syntaxe de mise à jour générique n’est pas la plus conviviale, vous devez faire preuve de patience.</span><span class="sxs-lookup"><span data-stu-id="6a45d-134">The generic update syntax isn't the most user friendly, so it will require some patience.</span></span>
2. <span data-ttu-id="6a45d-135">Vérifiez si le groupe `Generic Update Arguments` est exposé dans la commande de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="6a45d-135">Verify whether the update command has the `Generic Update Arguments` group exposed.</span></span> <span data-ttu-id="6a45d-136">Si ce n’est pas le cas, vous devez signaler un problème. Si c’est le cas, vous pouvez essayer de l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="6a45d-136">If not, you'll need to file an issue, but if they are you can attempt you scenario using them.</span></span>
3. <span data-ttu-id="6a45d-137">Utilisez la commande `show` sur la ressource qui vous intéresse pour déterminer le chemin à fournir dans les arguments génériques.</span><span class="sxs-lookup"><span data-stu-id="6a45d-137">Use the `show` command on the resource you are interested in to figure out what path you should supply in the generic arguments.</span></span> <span data-ttu-id="6a45d-138">Par exemple, avant d’essayer `az vm update`, exécutez `az vm show` pour identifier le chemin correct.</span><span class="sxs-lookup"><span data-stu-id="6a45d-138">For example, before you try out `az vm update`, run `az vm show` to determine the right path.</span></span> <span data-ttu-id="6a45d-139">En règle générale, vous allez utiliser la syntaxe à point pour accéder aux propriétés du dictionnaire et les crochets pour indexer dans des listes.</span><span class="sxs-lookup"><span data-stu-id="6a45d-139">Generally, you will use dot syntax to access dictionary properties and brackets to index into lists.</span></span>
4. <span data-ttu-id="6a45d-140">Consultez des exemples fonctionnels pour commencer.</span><span class="sxs-lookup"><span data-stu-id="6a45d-140">Check out working examples to get started.</span></span> <span data-ttu-id="6a45d-141">`az vm update -h` en contient d’excellents.</span><span class="sxs-lookup"><span data-stu-id="6a45d-141">`az vm update -h` has good ones.</span></span>
5. <span data-ttu-id="6a45d-142">`--set` et `--add` prennent une liste de paires clé-valeur au format `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-142">`--set` and `--add` take a list of key value pairs in the format of `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="6a45d-143">Utilisez-les pour construire des charges utiles complexes.</span><span class="sxs-lookup"><span data-stu-id="6a45d-143">Use them to construct non- trivial payloads.</span></span> <span data-ttu-id="6a45d-144">Si la syntaxe a trop de messages, envisagez d’utiliser une chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="6a45d-144">If the syntax gets too message, consider using a JSON string.</span></span> <span data-ttu-id="6a45d-145">Par exemple, pour attacher un nouveau disque de données à une machine virtuelle :</span><span class="sxs-lookup"><span data-stu-id="6a45d-145">For example, to attach a new data disk to a VM:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. <span data-ttu-id="6a45d-146">Il peut s’avérer plus utile de tirer parti de la convention `@{file}` de l’interface CLI, en plaçant le JSON dans un fichier et en le chargeant.</span><span class="sxs-lookup"><span data-stu-id="6a45d-146">You may find it more useful to leverage the CLI's `@{file}` convention, putting the JSON into a file and loading it.</span></span> <span data-ttu-id="6a45d-147">Cela simplifie la commande ci-dessus en :</span><span class="sxs-lookup"><span data-stu-id="6a45d-147">This simplifies the above command to:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a><span data-ttu-id="6a45d-148">Commandes de ressources génériques - `az resource`</span><span class="sxs-lookup"><span data-stu-id="6a45d-148">Generic resource commands - `az resource`</span></span>

<span data-ttu-id="6a45d-149">Il peut arriver qu’un service qui vous intéresse n’ait pas de couverture de commande d’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="6a45d-149">There may be cases where a service you are interested in does not have CLI command coverage.</span></span> <span data-ttu-id="6a45d-150">Vous pouvez employer les commandes `az resource create/show/list/delete/update/invoke-action` pour utiliser ces ressources.</span><span class="sxs-lookup"><span data-stu-id="6a45d-150">You can use the `az resource create/show/list/delete/update/invoke-action` commands to work with these resources.</span></span> <span data-ttu-id="6a45d-151">Voici quelques suggestions :</span><span class="sxs-lookup"><span data-stu-id="6a45d-151">Here are a few suggestions:</span></span>
1. <span data-ttu-id="6a45d-152">Si seules les commandes `create/update` sont impliquées, envisagez d’utiliser `az group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-152">If only `create/update` are involved, consider using `az group deployment create`.</span></span> <span data-ttu-id="6a45d-153">Mettez à profit les [modèles de démarrage rapide Microsoft Azure](https://github.com/Azure/azure-quickstart-templates) pour obtenir des exemples fonctionnels.</span><span class="sxs-lookup"><span data-stu-id="6a45d-153">Leverage [Azure Quickstart Templates](https://github.com/Azure/azure-quickstart-templates) for working examples.</span></span>
2. <span data-ttu-id="6a45d-154">Consultez les informations de référence sur l’API REST pour la charge utile de demande, l’URL et la version de l’API.</span><span class="sxs-lookup"><span data-stu-id="6a45d-154">Check out the Rest API reference for the request payload, URL and API version.</span></span> <span data-ttu-id="6a45d-155">À titre d’exemple, consultez les commentaires de la communauté sur [la façon de créer des ressources Application Insights](https://github.com/Azure/azure-cli/issues/5543).</span><span class="sxs-lookup"><span data-stu-id="6a45d-155">As an example, check out the community's comments on [how to create AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span></span>

## <a name="rest-api-command---az-rest"></a><span data-ttu-id="6a45d-156">Commande API REST - `az rest`</span><span class="sxs-lookup"><span data-stu-id="6a45d-156">REST API command - `az rest`</span></span>

<span data-ttu-id="6a45d-157">Si aucun argument de mise à jour générique ni `az resource` ne répond à vos besoins, vous pouvez utiliser la commande `az rest` pour appeler l’API REST.</span><span class="sxs-lookup"><span data-stu-id="6a45d-157">If neither generic update arguments nor `az resource` meets your needs, you can use `az rest` command to call the REST API.</span></span> <span data-ttu-id="6a45d-158">Elle s’authentifie automatiquement à l’aide des informations d’identification de connexion et définit l’en-tête `Content-Type: application/json`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-158">It automatically authenticates using the logged-in credential and sets header `Content-Type: application/json`.</span></span>

<span data-ttu-id="6a45d-159">Cela est très utile pour appeler l’[API Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) qui n’est pas prise en charge pour l’instant par les commandes d’interface CLI ([n°12946](https://github.com/Azure/azure-cli/issues/12946)).</span><span class="sxs-lookup"><span data-stu-id="6a45d-159">This is extremely useful for calling [Microsoft Graph API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) which is not currently supported by CLI commands ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span></span>

<span data-ttu-id="6a45d-160">Par exemple, pour mettre à jour `redirectUris` pour une [application](/graph/api/resources/application?view=graph-rest-1.0), nous appelons l’API REST [Mettre à jour l’application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) avec :</span><span class="sxs-lookup"><span data-stu-id="6a45d-160">For example, to update `redirectUris` for an [Application](/graph/api/resources/application?view=graph-rest-1.0), we call the [Update application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) REST API with:</span></span>

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

<span data-ttu-id="6a45d-161">Lorsque vous utilisez `--uri-parameters` pour les demandes sous la forme d’OData, veillez à placer `$` dans une séquence d’échappement dans différents environnements : dans `Bash`, placez `$` dans la séquence d’échappement `\$` et dans `PowerShell`, placez `$` dans la séquence `` `$``</span><span class="sxs-lookup"><span data-stu-id="6a45d-161">When using `--uri-parameters` for requests in the form of OData, please make sure to escape `$` in different environments: in `Bash`, escape `$` as `\$` and in `PowerShell`, escape `$` as `` `$``</span></span>

## <a name="quoting-issues"></a><span data-ttu-id="6a45d-162">Problèmes liés aux guillemets</span><span class="sxs-lookup"><span data-stu-id="6a45d-162">Quoting issues</span></span>

<span data-ttu-id="6a45d-163">Cela devient un problème car, lorsque l’interface de commande (Bash, Zsh, invite de commandes Windows, PowerShell, etc.) analyse la commande CLI, elle interprète les guillemets et les espaces.</span><span class="sxs-lookup"><span data-stu-id="6a45d-163">This becomes an issue because when the command shell (Bash, Zsh, Windows Command Prompt, PowerShell, etc) parses the CLI command, it will interpret the quotes and spaces.</span></span> <span data-ttu-id="6a45d-164">Reportez-vous toujours aux documents lorsque vous hésitez quant à l’utilisation d’un interpréteur de commandes :</span><span class="sxs-lookup"><span data-stu-id="6a45d-164">Always refer to the documents when you are uncertain about the usage of a shell:</span></span>

- <span data-ttu-id="6a45d-165">Bash : [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span><span class="sxs-lookup"><span data-stu-id="6a45d-165">Bash: [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span></span>
- <span data-ttu-id="6a45d-166">PowerShell : [À propos des règles liées aux guillemets](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span><span class="sxs-lookup"><span data-stu-id="6a45d-166">PowerShell: [About Quoting Rules](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span></span>
    - <span data-ttu-id="6a45d-167">En raison d’un problème connu ([n°1995](https://github.com/PowerShell/PowerShell/issues/1995)) de PowerShell, certaines règles d’échappement supplémentaires s’appliquent.</span><span class="sxs-lookup"><span data-stu-id="6a45d-167">Due to a known issue [#1995](https://github.com/PowerShell/PowerShell/issues/1995) of PowerShell, some extra escaping rules apply.</span></span> <span data-ttu-id="6a45d-168">Pour plus d’informations, consultez [Problèmes liés aux guillemets avec PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).</span><span class="sxs-lookup"><span data-stu-id="6a45d-168">See [Quoting issues with PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) for more information.</span></span>
- <span data-ttu-id="6a45d-169">Invite de commandes Windows : [Guide pratique pour placer dans une séquence d’échappement des caractères, délimiteurs et guillemets au niveau de la ligne de commande Windows](https://ss64.com/nt/syntax-esc.html)</span><span class="sxs-lookup"><span data-stu-id="6a45d-169">Windows Command Prompt: [How-to: Escape Characters, Delimiters and Quotes at the Windows command line](https://ss64.com/nt/syntax-esc.html)</span></span>

<span data-ttu-id="6a45d-170">Pour éviter des résultats imprévus, voici quelques suggestions :</span><span class="sxs-lookup"><span data-stu-id="6a45d-170">To avoid unanticipated results, here are a few suggestions:</span></span>

1. <span data-ttu-id="6a45d-171">Si la valeur contient un espace blanc, vous devez la wrapper entre guillemets.</span><span class="sxs-lookup"><span data-stu-id="6a45d-171">If the value contains whitespace, you must wrap it in quotes.</span></span>
2. <span data-ttu-id="6a45d-172">Dans Bash ou Windows PowerShell, les guillemets simples et doubles sont interprétés tandis que dans l’invite de commandes Windows, seuls les guillemets doubles sont gérés, ce qui signifie que les guillemets simples sont interprétés comme une partie de la valeur.</span><span class="sxs-lookup"><span data-stu-id="6a45d-172">In bash or Windows PowerShell, both single and double quotes will be interpreted, while in Windows Command Prompt, only double quotes are handled which means single quotes will be interpreted as a part of the value.</span></span>
3. <span data-ttu-id="6a45d-173">Si votre commande s’exécute uniquement sur Bash (ou Zsh), l’utilisation de guillemets simples présente l’avantage de conserver le contenu à l’intérieur.</span><span class="sxs-lookup"><span data-stu-id="6a45d-173">If your command only runs on Bash (or Zsh), using single quotes has the benefit of preserving the content inside.</span></span> <span data-ttu-id="6a45d-174">Cela peut être très utile lors de la fourniture de JSON inline.</span><span class="sxs-lookup"><span data-stu-id="6a45d-174">This can be very helpful when supplying inline JSON.</span></span> <span data-ttu-id="6a45d-175">Par exemple, la commande suivante fonctionne dans Bash : `'{"foo": "bar"}'`</span><span class="sxs-lookup"><span data-stu-id="6a45d-175">For example this works in bash: `'{"foo": "bar"}'`</span></span>
4. <span data-ttu-id="6a45d-176">Si votre commande s’exécute sur l’invite de commandes Windows, vous devez utiliser exclusivement des guillemets doubles.</span><span class="sxs-lookup"><span data-stu-id="6a45d-176">If your command will run on Windows Command Prompt, you must use double quotes exclusively.</span></span> <span data-ttu-id="6a45d-177">Si la valeur contient des guillemets doubles, vous devez la placer dans une séquence d’échappement : `"i like to use \" a lot"`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-177">If the value contains double quotes, you must escape it: `"i like to use \" a lot"`.</span></span> <span data-ttu-id="6a45d-178">L’équivalent pour l’invite de commandes de la commande ci-dessus est : `"{\"foo\": \"bar\"}"`</span><span class="sxs-lookup"><span data-stu-id="6a45d-178">The Command Prompt equivalent of the above would be: `"{\"foo\": \"bar\"}"`</span></span>
5. <span data-ttu-id="6a45d-179">Les variables exportées dans Bash entre guillemets doubles sont évaluées.</span><span class="sxs-lookup"><span data-stu-id="6a45d-179">Exported variables in bash inside double quotes will be evaluated.</span></span> <span data-ttu-id="6a45d-180">Si ce n’est pas ce que vous voulez, utilisez de nouveau `\ ` pour placer la valeur dans une séquence d’échappement comme `"\$var"` ou utilisez des guillemets simples `'$var'`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-180">If this is not what you want, again use `\ ` to escape it like `"\$var"` or use single quotes `'$var'`.</span></span>
6. <span data-ttu-id="6a45d-181">Quelques arguments CLI, dont les arguments de mise à jour génériques, prennent une liste de valeurs séparées par des espaces, comme `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-181">A few CLI arguments, including the generic update arguments, take a list of space-separated values, like `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="6a45d-182">Étant donné que le nom de la clé et la valeur peuvent accepter une chaîne arbitraire susceptible de contenir un espace blanc, l’utilisation de guillemets est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="6a45d-182">Since the key name and value can take arbitrary string which might contain whitespace, using quotes will be necessary.</span></span> <span data-ttu-id="6a45d-183">Wrappez la paire, et non la clé ou la valeur individuelle.</span><span class="sxs-lookup"><span data-stu-id="6a45d-183">Wrap the pair, not individual key or value.</span></span> <span data-ttu-id="6a45d-184">`"my name"=john` est donc incorrect.</span><span class="sxs-lookup"><span data-stu-id="6a45d-184">So `"my name"=john` is wrong.</span></span> <span data-ttu-id="6a45d-185">Utilisez plutôt `"my name=john"`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-185">Instead, use `"my name=john"`.</span></span> <span data-ttu-id="6a45d-186">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="6a45d-186">For example:</span></span>
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. <span data-ttu-id="6a45d-187">Utilisez la convention `@<file>` de l’interface CLI pour le chargement à partir d’un fichier afin de contourner les mécanismes d’interprétation de l’interpréteur de commandes :</span><span class="sxs-lookup"><span data-stu-id="6a45d-187">Use CLI's `@<file>` convention to load from a file so to bypass the shell's interpretation mechanisms:</span></span>
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. <span data-ttu-id="6a45d-188">Lorsqu’un argument CLI indique qu’il accepte une liste de valeurs séparées par des espaces, les formats acceptés sont les suivants :</span><span class="sxs-lookup"><span data-stu-id="6a45d-188">When a CLI argument says it accepts a space-separated list, these are the formats accepted:</span></span>
    - <span data-ttu-id="6a45d-189">`--arg foo bar`: OK.</span><span class="sxs-lookup"><span data-stu-id="6a45d-189">`--arg foo bar`: OK.</span></span> <span data-ttu-id="6a45d-190">Liste de valeurs séparées par des espaces, sans guillemets</span><span class="sxs-lookup"><span data-stu-id="6a45d-190">Unquoted, space-separated list</span></span>
    - <span data-ttu-id="6a45d-191">`--arg "foo" "bar"`: OK : Liste de valeurs séparées par des espaces, avec guillemets</span><span class="sxs-lookup"><span data-stu-id="6a45d-191">`--arg "foo" "bar"`: OK: Quoted, space-separated list</span></span>
    - <span data-ttu-id="6a45d-192">`--arg "foo bar"`: BAD.</span><span class="sxs-lookup"><span data-stu-id="6a45d-192">`--arg "foo bar"`: BAD.</span></span> <span data-ttu-id="6a45d-193">Il s’agit d’une chaîne contenant un espace et non d’une liste de valeurs séparées par des espaces.</span><span class="sxs-lookup"><span data-stu-id="6a45d-193">This is a string with a space in it, not a space-separated list.</span></span>
9. <span data-ttu-id="6a45d-194">Lors de l’exécution de commandes Azure CLI dans PowerShell, l’analyse des erreurs se produit quand les arguments contiennent des caractères spéciaux de PowerShell, comme `@`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-194">When running Azure CLI commands in PowerShell, parsing errors will occur when the arguments contain special characters of PowerShell, such as at `@`.</span></span> <span data-ttu-id="6a45d-195">Vous pouvez résoudre ce problème en ajoutant `` ` `` avant le caractère spécial pour le placer dans une séquence d’échappement, ou en mettant l’argument entre guillemets simples ou doubles `'`/`"`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-195">You can solve this problem by adding `` ` `` before the special character to escape it, or by enclosing the argument with single or double quotes `'`/`"`.</span></span> <span data-ttu-id="6a45d-196">Par exemple, `az group deployment create --parameters @parameters.json` ne fonctionne pas dans PowerShell, car `@` est analysé en tant que [symbole de projection](/powershell/module/microsoft.powershell.core/about/about_splatting).</span><span class="sxs-lookup"><span data-stu-id="6a45d-196">For example, `az group deployment create --parameters @parameters.json` doesn't work in PowerShell because `@` is parsed as a [splatting symbol](/powershell/module/microsoft.powershell.core/about/about_splatting).</span></span> <span data-ttu-id="6a45d-197">Pour résoudre ce problème, vous pouvez remplacer l’argument par `` `@parameters.json`` ou `'@parameters.json'`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-197">To fix this, you may change the argument to `` `@parameters.json`` or `'@parameters.json'`.</span></span>
10. <span data-ttu-id="6a45d-198">Lorsque vous utilisez `--query` avec une commande, certains caractères de [JMESPath](https://jmespath.org/specification.html) doivent être placés dans une séquence d’échappement dans l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="6a45d-198">When using `--query` with a command, some characters of [JMESPath](https://jmespath.org/specification.html) need to be escaped in the shell.</span></span> <span data-ttu-id="6a45d-199">Par exemple, dans Bash :</span><span class="sxs-lookup"><span data-stu-id="6a45d-199">For example, in Bash:</span></span>
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

    <span data-ttu-id="6a45d-200">Dans l’invite de commandes :</span><span class="sxs-lookup"><span data-stu-id="6a45d-200">In Command Prompt:</span></span>
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    <span data-ttu-id="6a45d-201">Dans PowerShell (des séquences d’échappement supplémentaires sont nécessaires) :</span><span class="sxs-lookup"><span data-stu-id="6a45d-201">In PowerShell (extra escaping is needed):</span></span>
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

11. <span data-ttu-id="6a45d-202">La meilleure façon de résoudre un problème lié aux guillemets consiste à exécuter la commande avec l’indicateur `--debug`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-202">The best way to troubleshoot a quoting issue is to run the command with `--debug` flag.</span></span> <span data-ttu-id="6a45d-203">Il révèle les arguments réels reçus par l’interface CLI dans la [syntaxe de Python](https://docs.python.org/3/tutorial/introduction.html#strings).</span><span class="sxs-lookup"><span data-stu-id="6a45d-203">It reveals the actual arguments received by CLI in [Python's syntax](https://docs.python.org/3/tutorial/introduction.html#strings).</span></span> <span data-ttu-id="6a45d-204">Par exemple, dans Bash :</span><span class="sxs-lookup"><span data-stu-id="6a45d-204">For example, in Bash:</span></span>

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

## <a name="work-behind-a-proxy"></a><span data-ttu-id="6a45d-205">Travail derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="6a45d-205">Work behind a proxy</span></span>

<span data-ttu-id="6a45d-206">Le proxy est courant derrière le réseau d’entreprise ou introduit par des outils de suivi tels que Fiddler, mitmproxy, etc. Si le proxy utilise des certificats auto-signés, la bibliothèque de [demandes](https://github.com/kennethreitz/requests) de Python que l’interface CLI utilise va générer `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-206">Proxy is common behind corporate network or introduced by tracing tools like Fiddler, mitmproxy, etc. If the proxy uses self-signed certificates, the Python [Requests](https://github.com/kennethreitz/requests) library which CLI uses will throw `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span></span> <span data-ttu-id="6a45d-207">Il existe 2 moyens de gérer cette erreur :</span><span class="sxs-lookup"><span data-stu-id="6a45d-207">There are 2 ways to handle this error:</span></span>

1. <span data-ttu-id="6a45d-208">Définissez la variable d’environnement `REQUESTS_CA_BUNDLE` sur le chemin du fichier du certificat de groupement d’autorités de certification au format PEM.</span><span class="sxs-lookup"><span data-stu-id="6a45d-208">Set environment variable `REQUESTS_CA_BUNDLE` to the path of CA bundle certificate file in PEM format.</span></span> <span data-ttu-id="6a45d-209">Cette option est recommandée si vous utilisez l’interface CLI fréquemment derrière un proxy d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="6a45d-209">This is recommended if you use CLI frequently behind a corporate proxy.</span></span> <span data-ttu-id="6a45d-210">Le groupement d’autorités de certification par défaut utilisé par l’interface CLI se trouve sur `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` sur Windows et ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` sur Linux.</span><span class="sxs-lookup"><span data-stu-id="6a45d-210">The default CA bundle which CLI uses is located at `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` on Windows and ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` on Linux.</span></span> <span data-ttu-id="6a45d-211">Vous pouvez ajouter le certificat du serveur proxy à ce fichier ou copier le contenu dans un autre fichier de certificat, puis définir `REQUESTS_CA_BUNDLE` sur celui-ci.</span><span class="sxs-lookup"><span data-stu-id="6a45d-211">You may append the proxy server's certificate to this file or copy the contents to another certificate file, then set `REQUESTS_CA_BUNDLE` to it.</span></span> <span data-ttu-id="6a45d-212">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="6a45d-212">For example:</span></span>

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   <span data-ttu-id="6a45d-213">Il est fréquemment demandé si les variables d’environnement `HTTP_PROXY` ou `HTTPS_PROXY` doivent ou non être définies, et la réponse est que cela dépend.</span><span class="sxs-lookup"><span data-stu-id="6a45d-213">A frequent ask is whether or not `HTTP_PROXY` or `HTTPS_PROXY` environment variables should be set, the answer is it depends.</span></span> <span data-ttu-id="6a45d-214">Pour Fiddler sur Windows, la variable agit par défaut en tant que proxy système au démarrage et vous n’avez pas besoin de définir quoi que ce soit.</span><span class="sxs-lookup"><span data-stu-id="6a45d-214">For Fiddler on Windows, by default it acts as system proxy on start, you don't need to set anything.</span></span> <span data-ttu-id="6a45d-215">Si l’option est désactivée ou que vous utilisez d’autres outils qui ne fonctionnent pas en tant que proxy système, vous devez les définir.</span><span class="sxs-lookup"><span data-stu-id="6a45d-215">If the option is off or using other tools which don't work as system proxy, you should set them.</span></span> <span data-ttu-id="6a45d-216">Comme presque tout le trafic de l’interface CLI est basé sur SSL, seule `HTTPS_PROXY` doit être définie.</span><span class="sxs-lookup"><span data-stu-id="6a45d-216">Since almost all traffic from CLI is SSL-based, only `HTTPS_PROXY` should be set.</span></span> <span data-ttu-id="6a45d-217">Si vous ne savez pas, il vous suffit de les définir, mais n’oubliez pas d’annuler cette configuration après l’arrêt du proxy.</span><span class="sxs-lookup"><span data-stu-id="6a45d-217">If you are not sure, just set them, but do remember to unset it after the proxy is shut down.</span></span> <span data-ttu-id="6a45d-218">Pour Fiddler, la valeur par défaut est `http://localhost:8888`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-218">For fiddler, the default value is `http://localhost:8888`.</span></span>

   <span data-ttu-id="6a45d-219">Pour plus d’informations, consultez le [blog de Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span><span class="sxs-lookup"><span data-stu-id="6a45d-219">For other details, check out [Stefan's blog](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span></span>

2. <span data-ttu-id="6a45d-220">Désactivez la vérification du certificat sur Azure CLI en définissant la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-220">Disable the certificate check across Azure CLI by setting environment variable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span></span> <span data-ttu-id="6a45d-221">Cette solution n’est pas sûre, mais elle est valable pendant une brève période comme la capture d’une trace réseau pour une commande spécifique. Il convient de désactiver cette option rapidement une fois l’opération terminée.</span><span class="sxs-lookup"><span data-stu-id="6a45d-221">This is not safe, but good for a short period like capturing a network trace for a specific command and promptly turning it off when finished.</span></span> <span data-ttu-id="6a45d-222">Cela peut ne pas fonctionner pour certaines commandes de plan de données en raison des limitations du SDK sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="6a45d-222">This may not work for some data-plane commands due to underlying SDK limitations.</span></span>

## <a name="concurrent-builds"></a><span data-ttu-id="6a45d-223">Builds simultanées</span><span class="sxs-lookup"><span data-stu-id="6a45d-223">Concurrent builds</span></span>

<span data-ttu-id="6a45d-224">Si vous utilisez az sur un ordinateur de build et que plusieurs travaux peuvent être exécutés en parallèle, il existe un risque que les jetons de connexion soient partagés entre deux travaux de build si les travaux sont exécutés sous le même nom d’utilisateur du système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="6a45d-224">If you are using az on a build machine, and multiple jobs can be run in parallel, then there is a risk that the login tokens are shared between two build jobs is the jobs run as the same OS user.</span></span>  <span data-ttu-id="6a45d-225">Pour éviter une telle confusion, définissez AZURE_CONFIG_DIR sur un répertoire dans lequel les jetons de connexion doivent être stockés.</span><span class="sxs-lookup"><span data-stu-id="6a45d-225">To avoid mix ups like this, set AZURE_CONFIG_DIR to a directory where the login tokens should be stored.</span></span>  <span data-ttu-id="6a45d-226">Il peut s’agir d’un dossier créé de manière aléatoire, ou simplement du nom de l’espace de travail Jenkins, comme suit : ```AZURE_CONFIG_DIR=.```</span><span class="sxs-lookup"><span data-stu-id="6a45d-226">It could be a randomly created folder, or just the name of the jenkins workspace, like this ```AZURE_CONFIG_DIR=.```</span></span>

## <a name="appendix"></a><span data-ttu-id="6a45d-227">Annexe</span><span class="sxs-lookup"><span data-stu-id="6a45d-227">Appendix</span></span>

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="6a45d-228">Scripts de commandes par lot Windows pour l’enregistrement dans des variables et une utilisation ultérieure</span><span class="sxs-lookup"><span data-stu-id="6a45d-228">Windows batch scripts for saving to variables and using it later</span></span>

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="6a45d-229">Scripts Windows PowerShell pour l’enregistrement dans des variables et une utilisation ultérieure</span><span class="sxs-lookup"><span data-stu-id="6a45d-229">Windows PowerShell scripts for saving to variables and using it later</span></span>

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a><span data-ttu-id="6a45d-230">Scripts de commandes par lot Windows pour parcourir une liste</span><span class="sxs-lookup"><span data-stu-id="6a45d-230">Windows batch scripts to loop through a list</span></span>
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a><span data-ttu-id="6a45d-231">Scripts Windows PowerShell pour parcourir une liste</span><span class="sxs-lookup"><span data-stu-id="6a45d-231">Windows PowerShell scripts to loop through a list</span></span>
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a><span data-ttu-id="6a45d-232">Variables d’environnement CLI</span><span class="sxs-lookup"><span data-stu-id="6a45d-232">CLI Environment Variables</span></span>

|  <span data-ttu-id="6a45d-233">Variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="6a45d-233">Environment Variable</span></span>          | <span data-ttu-id="6a45d-234">Description</span><span class="sxs-lookup"><span data-stu-id="6a45d-234">Description</span></span>            |
|--------------------------------|------------------------|
| <span data-ttu-id="6a45d-235">**AZURE_CONFIG_DIR**</span><span class="sxs-lookup"><span data-stu-id="6a45d-235">**AZURE_CONFIG_DIR**</span></span>           | <span data-ttu-id="6a45d-236">Répertoire de configuration globale pour les fichiers de configuration, les journaux et la télémétrie.</span><span class="sxs-lookup"><span data-stu-id="6a45d-236">Global config directory for config files, logs and telemetry.</span></span> <span data-ttu-id="6a45d-237">Si elle n’est pas spécifiée, la valeur par défaut est `~/.azure`.</span><span class="sxs-lookup"><span data-stu-id="6a45d-237">If unspecified, defaults to `~/.azure`.</span></span> |
| <span data-ttu-id="6a45d-238">**AZURE_EXTENSION_DIR**</span><span class="sxs-lookup"><span data-stu-id="6a45d-238">**AZURE_EXTENSION_DIR**</span></span>        | <span data-ttu-id="6a45d-239">Répertoire d’installation des extensions.</span><span class="sxs-lookup"><span data-stu-id="6a45d-239">Extensions' installation directory.</span></span> <span data-ttu-id="6a45d-240">Si elle n’est pas spécifiée, la valeur par défaut est le répertoire `cliextensions` dans le répertoire de configuration globale.</span><span class="sxs-lookup"><span data-stu-id="6a45d-240">If unspecified, defaults to `cliextensions` directory within the global config directory.</span></span> |
