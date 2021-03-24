---
title: Options des paramètres persistants Azure CLI
description: Comment utiliser des paramètres persistants Azure CLI pour stocker des valeurs de paramètre réutilisables
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 128847cb14b48fef326859eb77aab9e66e88b6fd
ms.sourcegitcommit: 936ec07eb1c56e24d8000cc24a2a0e05102e0cf4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "104928796"
---
# <a name="azure-cli-persisted-parameter"></a><span data-ttu-id="81be6-103">Paramètre persistant Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81be6-103">Azure CLI persisted parameter</span></span>

<span data-ttu-id="81be6-104">La référence Azure CLI [az config param-persist](/cli/azure/config/param-persist) permet de conserver les valeurs de paramètres persistants en local pour des commandes Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81be6-104">The Azure CLI [az config param-persist](/cli/azure/config/param-persist) reference provides the ability to retain local persisted parameter values for Azure CLI commands.</span></span>  <span data-ttu-id="81be6-105">Cela évite de devoir retaper continuellement des paramètres couramment utilisés.</span><span class="sxs-lookup"><span data-stu-id="81be6-105">This removes the need to continually retype common parameters.</span></span> <span data-ttu-id="81be6-106">Par exemple, les paramètres location et resource-group sont obligatoires dans de nombreuses commandes CLI, mais ils ne contribuent pas à l’_intention_ de la commande.</span><span class="sxs-lookup"><span data-stu-id="81be6-106">For example, location and resource-group are required parameters in many CLI commands, but they don't contribute to the _intent_ of the command.</span></span>  <span data-ttu-id="81be6-107">Quand vous stockez les valeurs de paramètres persistants, vous réduisez la redondance et pouvez écourter considérablement la syntaxe des commandes CLI.</span><span class="sxs-lookup"><span data-stu-id="81be6-107">When you store parameter values with persisted parameter, you reduce redundancy and can significantly shorten CLI command syntax.</span></span>

<span data-ttu-id="81be6-108">Les valeurs de configuration utilisées par l’interface CLI sont évaluées dans l’ordre suivant. Les éléments situés en haut de la liste sont prioritaires.</span><span class="sxs-lookup"><span data-stu-id="81be6-108">Configuration values used by the CLI are evaluated in the following precedence, with items higher on the list taking priority.</span></span>

1. <span data-ttu-id="81be6-109">Paramètres de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="81be6-109">Command-line parameters</span></span>
1. <span data-ttu-id="81be6-110">Valeurs dans le répertoire de travail local définies par `az config param-persist`</span><span class="sxs-lookup"><span data-stu-id="81be6-110">Values in the local working directory set by `az config param-persist`</span></span>
1. <span data-ttu-id="81be6-111">Variables d'environnement</span><span class="sxs-lookup"><span data-stu-id="81be6-111">Environment variables</span></span>
1. <span data-ttu-id="81be6-112">Valeurs du fichier de configuration ou définies avec `az config`</span><span class="sxs-lookup"><span data-stu-id="81be6-112">Values in the configuration file or set with `az config`</span></span>

<span data-ttu-id="81be6-113">[Installez Azure CLI](install-azure-cli.md) ou ouvrez [Azure Cloud Shell](https://shell.azure.com) pour exécuter les scripts de cet article.</span><span class="sxs-lookup"><span data-stu-id="81be6-113">[Install the Azure CLI](install-azure-cli.md) or open [Azure Cloud Shell](https://shell.azure.com) to run the scripts in this article.</span></span>  <span data-ttu-id="81be6-114">Si vous utilisez une installation locale d’Azure CLI, la version 2.12.0 ou ultérieure est nécessaire pour exécuter les commandes `az config param-persist`.</span><span class="sxs-lookup"><span data-stu-id="81be6-114">If you are using a local install of the Azure CLI, version 2.12.0 or later is needed to run `az config param-persist` commands.</span></span>  <span data-ttu-id="81be6-115">Exécutez [az version](/cli/azure/reference-index#az_version) pour rechercher la version et les bibliothèques dépendantes installées.</span><span class="sxs-lookup"><span data-stu-id="81be6-115">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="81be6-116">Pour effectuer une mise à niveau vers la dernière version, exécutez [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="81be6-116">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>  <span data-ttu-id="81be6-117">Azure Cloud Shell dispose toujours de la dernière version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81be6-117">Azure Cloud Shell always has the latest version of the Azure CLI.</span></span>

## <a name="persisted-parameter-data-file"></a><span data-ttu-id="81be6-118">Fichier de données des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="81be6-118">Persisted parameter data file</span></span>

<span data-ttu-id="81be6-119">Les valeurs des paramètres persistants sont conservées dans un fichier nommé `.param_persist` qui est stocké dans votre répertoire de travail.</span><span class="sxs-lookup"><span data-stu-id="81be6-119">Persisted parameter values are kept in a file named `.param_persist` which is stored in your working directory.</span></span>  <span data-ttu-id="81be6-120">Si vous utilisez [Azure Cloud Shell](https://shell.azure.com) pour exécuter des commandes Azure CLI, votre répertoire de travail se trouve dans le compte de stockage utilisé par Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="81be6-120">If you are using [Azure Cloud Shell](https://shell.azure.com) to execute Azure CLI commands, your working directory is in the storage account being used by the Azure CLI.</span></span>  <span data-ttu-id="81be6-121">Si vous utilisez une [installation locale](install-azure-cli.md) d’Azure CLI, votre répertoire de travail se trouve sur votre ordinateur local.</span><span class="sxs-lookup"><span data-stu-id="81be6-121">If you are using a [local install](install-azure-cli.md) of the Azure CLI, your working directory is on your local machine.</span></span>  <span data-ttu-id="81be6-122">Dans les deux cas, le fichier `.param_persist` est masqué et ne doit pas être mis à jour manuellement.</span><span class="sxs-lookup"><span data-stu-id="81be6-122">In either location, the `.param_persist` file is hidden and should not be manually updated.</span></span>

## <a name="persisted-parameter-storage-and-support"></a><span data-ttu-id="81be6-123">Stockage et prise en charge des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="81be6-123">Persisted parameter storage and support</span></span>

<span data-ttu-id="81be6-124">Les paramètres Azure CLI suivants sont pris en charge par le paramètre persistant.</span><span class="sxs-lookup"><span data-stu-id="81be6-124">The following Azure CLI parameters are supported by persisted parameter.</span></span>  <span data-ttu-id="81be6-125">Les paramètres `resource_group_name` et `location` sont stockés différemment, ce qui vous permet de les ajouter au paramètre persistant _sans_ exécuter de commande create.</span><span class="sxs-lookup"><span data-stu-id="81be6-125">The `resource_group_name` and `location` parameters are stored differently in that you can add them to persisted parameter _without_ executing a create command.</span></span>

| <span data-ttu-id="81be6-126">Paramètre persistant</span><span class="sxs-lookup"><span data-stu-id="81be6-126">Persisted parameter</span></span> | <span data-ttu-id="81be6-127">Action de stockage</span><span class="sxs-lookup"><span data-stu-id="81be6-127">Storage action</span></span> | <span data-ttu-id="81be6-128">Pris en charge par</span><span class="sxs-lookup"><span data-stu-id="81be6-128">Supported by</span></span>
|-|-|-|
| <span data-ttu-id="81be6-129">location</span><span class="sxs-lookup"><span data-stu-id="81be6-129">location</span></span> | <span data-ttu-id="81be6-130">Exécuter n’importe quelle commande</span><span class="sxs-lookup"><span data-stu-id="81be6-130">Execute any command</span></span> | <span data-ttu-id="81be6-131">Toutes les références Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81be6-131">All Azure CLI references</span></span>
| <span data-ttu-id="81be6-132">resource_group_name</span><span class="sxs-lookup"><span data-stu-id="81be6-132">resource_group_name</span></span> | <span data-ttu-id="81be6-133">Exécuter n’importe quelle commande</span><span class="sxs-lookup"><span data-stu-id="81be6-133">Execute any command</span></span> | <span data-ttu-id="81be6-134">Toutes les références Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81be6-134">All Azure CLI references</span></span>
| <span data-ttu-id="81be6-135">vnet_name</span><span class="sxs-lookup"><span data-stu-id="81be6-135">vnet_name</span></span> | <span data-ttu-id="81be6-136">Exécuter une commande create</span><span class="sxs-lookup"><span data-stu-id="81be6-136">Execute a create command</span></span> | <span data-ttu-id="81be6-137">Azure Web Apps uniquement</span><span class="sxs-lookup"><span data-stu-id="81be6-137">Azure Web Apps only</span></span>
| <span data-ttu-id="81be6-138">storage_account_name</span><span class="sxs-lookup"><span data-stu-id="81be6-138">storage_account_name</span></span> | <span data-ttu-id="81be6-139">Exécuter une commande create</span><span class="sxs-lookup"><span data-stu-id="81be6-139">Execute a create command</span></span> |  <span data-ttu-id="81be6-140">Azure Web Apps uniquement</span><span class="sxs-lookup"><span data-stu-id="81be6-140">Azure Web Apps only</span></span>
| <span data-ttu-id="81be6-141">webapp_name</span><span class="sxs-lookup"><span data-stu-id="81be6-141">webapp_name</span></span> | <span data-ttu-id="81be6-142">Exécuter une commande create</span><span class="sxs-lookup"><span data-stu-id="81be6-142">Execute a create command</span></span> | <span data-ttu-id="81be6-143">Azure Web Apps uniquement</span><span class="sxs-lookup"><span data-stu-id="81be6-143">Azure Web Apps only</span></span>
| <span data-ttu-id="81be6-144">function_app_name</span><span class="sxs-lookup"><span data-stu-id="81be6-144">function_app_name</span></span> | <span data-ttu-id="81be6-145">Exécuter une commande create</span><span class="sxs-lookup"><span data-stu-id="81be6-145">Execute a create command</span></span> | <span data-ttu-id="81be6-146">Azure Functions uniquement</span><span class="sxs-lookup"><span data-stu-id="81be6-146">Azure Functions only</span></span>

## <a name="sample-script-using-persisted-parameters"></a><span data-ttu-id="81be6-147">Exemple de script utilisant des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="81be6-147">Sample script using persisted parameters</span></span>

<span data-ttu-id="81be6-148">Sans paramètres persistants, les commandes CLI séquentielles doivent répéter les mêmes valeurs de paramètres.</span><span class="sxs-lookup"><span data-stu-id="81be6-148">Without persisted parameters, sequential CLI commands must repeat the same parameter values.</span></span>  <span data-ttu-id="81be6-149">Quand les paramètres persistants sont activés, les valeurs stockées de vos paramètres peuvent être omises des commandes séquentielles.</span><span class="sxs-lookup"><span data-stu-id="81be6-149">With persisted parameters enabled, your stored parameter values can be omitted from sequential commands.</span></span>  <span data-ttu-id="81be6-150">Dans cet exemple, l’`location`, le `resource group name` et le `storage account name` sont répétés dans les commandes suivantes.</span><span class="sxs-lookup"><span data-stu-id="81be6-150">In this example, the `location`, `resource group name` or `storage account name` are repeated in subsequent commands.</span></span>

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a><span data-ttu-id="81be6-151">Comparaison des paramètres persistants et des variables globales</span><span class="sxs-lookup"><span data-stu-id="81be6-151">Persisted parameter and global variable comparison</span></span>

<span data-ttu-id="81be6-152">Deux commandes Azure CLI peuvent être utilisées pour définir les valeurs par défaut de paramètres : `az configure` et `az config param-persist`.</span><span class="sxs-lookup"><span data-stu-id="81be6-152">There are two Azure CLI commands that can be used to default parameter values: `az configure` and `az config param-persist`.</span></span>  <span data-ttu-id="81be6-153">Utilisez la commande `az configure` pour spécifier des _variables globales_ telles que le groupe, l’emplacement ou le web.</span><span class="sxs-lookup"><span data-stu-id="81be6-153">Use the `az configure` command to specify _global variables_ such as group, location, or web.</span></span>  <span data-ttu-id="81be6-154">Utilisez `az param-persist` pour spécifier des _valeurs locales par défaut_ propres à votre charge de travail.</span><span class="sxs-lookup"><span data-stu-id="81be6-154">Use `az param-persist` to specify _local default values_ unique to your workload.</span></span>  <span data-ttu-id="81be6-155">Les valeurs stockées sont utilisées par CLI à la place des arguments obligatoires.</span><span class="sxs-lookup"><span data-stu-id="81be6-155">Stored values are used by the CLI in place of required arguments.</span></span>

> [!Important]
> <span data-ttu-id="81be6-156">Les paramètres persistants remplacent les valeurs de contexte globales.</span><span class="sxs-lookup"><span data-stu-id="81be6-156">Persisted parameters override global context values.</span></span>
>

| <span data-ttu-id="81be6-157">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="81be6-157">Reference</span></span> | <span data-ttu-id="81be6-158">Étendue</span><span class="sxs-lookup"><span data-stu-id="81be6-158">Scope</span></span> | <span data-ttu-id="81be6-159">Définissez</span><span class="sxs-lookup"><span data-stu-id="81be6-159">Set</span></span> | <span data-ttu-id="81be6-160">Utilisation</span><span class="sxs-lookup"><span data-stu-id="81be6-160">Use</span></span>
|-|-|-|-|
[<span data-ttu-id="81be6-161">az configure</span><span class="sxs-lookup"><span data-stu-id="81be6-161">az configure</span></span>](/cli/azure/reference-index#az_configure) | <span data-ttu-id="81be6-162">Étendue globale à l’échelle de CLI</span><span class="sxs-lookup"><span data-stu-id="81be6-162">Scoped globally across the CLI</span></span> | <span data-ttu-id="81be6-163">Définition explicite avec `az configure --defaults`</span><span class="sxs-lookup"><span data-stu-id="81be6-163">Set explicitly using `az configure --defaults`</span></span> | <span data-ttu-id="81be6-164">Utilisation avec des paramètres liés à la journalisation, la collecte de données et les valeurs d’argument par défaut.</span><span class="sxs-lookup"><span data-stu-id="81be6-164">Use for settings such as logging, data collection, and default argument values</span></span>
[<span data-ttu-id="81be6-165">az config param-persist</span><span class="sxs-lookup"><span data-stu-id="81be6-165">az config param-persist</span></span>](/cli/azure/config/param-persist) | <span data-ttu-id="81be6-166">Étendue locale à l’échelle d’un répertoire de travail spécifique</span><span class="sxs-lookup"><span data-stu-id="81be6-166">Scoped locally to a specific working directory</span></span> | <span data-ttu-id="81be6-167">Définition automatique une fois les paramètres persistants activés</span><span class="sxs-lookup"><span data-stu-id="81be6-167">Set automatically once persisted parameters are turned on</span></span> | <span data-ttu-id="81be6-168">Utilisation pour des commandes séquentielles de charges de travail individuelles.</span><span class="sxs-lookup"><span data-stu-id="81be6-168">Use for individual workload sequential commands.</span></span>

### <a name="command-examples"></a><span data-ttu-id="81be6-169">Exemples de commandes</span><span class="sxs-lookup"><span data-stu-id="81be6-169">Command examples</span></span>

<span data-ttu-id="81be6-170">Utilisez `az config param-persist` pour définir une variable globale utilisée dans le cadre de la création d’un compte de stockage Azure.</span><span class="sxs-lookup"><span data-stu-id="81be6-170">Use `az config param-persist` to set a global variable used in the creation of an Azure storage account.</span></span>

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="81be6-171">La sortie de la commande CLI montre qu’un compte de stockage a été créé dans le groupe de ressources trouvé dans la variable globale « myGlobalVariableRG ».</span><span class="sxs-lookup"><span data-stu-id="81be6-171">CLI command output shows that a new storage account was created in the resource group found in the global variable, \`myGlobalVariableRG'.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

<span data-ttu-id="81be6-172">Utilisez `az config param-persist` pour définir les paramètres persistants utilisés dans le cadre de la création d’un compte de stockage Azure.</span><span class="sxs-lookup"><span data-stu-id="81be6-172">Use `az config param-persist` to set persisted parameters used in the creation of an Azure storage account.</span></span>  <span data-ttu-id="81be6-173">Si une variable globale est définie pour le même objet, le paramètre persistant remplace la variable globale.</span><span class="sxs-lookup"><span data-stu-id="81be6-173">If a global variable is set for the same object, the persisted parameter will override the global variable.</span></span>

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="81be6-174">Même avec une variable globale définie pour un groupe de ressources avec la valeur `myGlobalVariableRG`, le compte de stockage est créé avec `myParamPersistRG` si les paramètres persistants sont activés.</span><span class="sxs-lookup"><span data-stu-id="81be6-174">Even with a global variable set for resource group with a value of `myGlobalVariableRG`, with persisted parameters turned on, the new storage account was created with `myParamPersistRG`.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a><span data-ttu-id="81be6-175">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81be6-175">See also</span></span>

* [<span data-ttu-id="81be6-176">Tutoriel : Utiliser des paramètres persistants avec des commandes Azure CLI séquentielles</span><span class="sxs-lookup"><span data-stu-id="81be6-176">Tutorial: Use persisted parameter with sequential Azure CLI commands</span></span>](param-persist-tutorial.md)
* [<span data-ttu-id="81be6-177">Configuration d’Azure CLI avec az configure</span><span class="sxs-lookup"><span data-stu-id="81be6-177">Azure CLI Configuration using az configure</span></span>](azure-cli-configuration.md)
