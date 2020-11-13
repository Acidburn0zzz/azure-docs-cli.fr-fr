---
title: Tutoriel sur l’utilisation de paramètres persistants avec Azure CLI
description: Tutoriel sur l’utilisation de la commande az config param-persist pour stocker les valeurs de paramètres Azure CLI en vue d’une utilisation répétée
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 49bf1d852f000dfbe6251cc15bd63e780b3bc91a
ms.sourcegitcommit: 8d514f4147d6edfc02d8d95d5a4243d100a7fcc9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2020
ms.locfileid: "93423189"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a><span data-ttu-id="986da-103">Tutoriel : Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles</span><span class="sxs-lookup"><span data-stu-id="986da-103">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>

<span data-ttu-id="986da-104">Azure CLI offre des paramètres persistants qui vous permettent de stocker les valeurs de paramètres en vue d’une utilisation continue.</span><span class="sxs-lookup"><span data-stu-id="986da-104">Azure CLI offers persisted parameters that enable you to store parameter values for continued use.</span></span>  <span data-ttu-id="986da-105">Dans ce tutoriel, vous allez apprendre à vous servir de valeurs persistantes et à utiliser ces valeurs locales pour exécuter efficacement des commandes séquentielles.</span><span class="sxs-lookup"><span data-stu-id="986da-105">In this tutorial, you learn how to work with persisted values, and use these local values to efficiently execute sequential commands.</span></span>

<span data-ttu-id="986da-106">Ce didacticiel vous apprendra à effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="986da-106">In this tutorial, you will learn to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="986da-107">Utiliser des commandes de référence **az config param-persist**</span><span class="sxs-lookup"><span data-stu-id="986da-107">Use **az config param-persist** reference commands</span></span>
> * <span data-ttu-id="986da-108">Exécuter des commandes séquentielles à l’aide de paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-108">Execute sequential commands using persisted parameters</span></span>

<span data-ttu-id="986da-109">Ce tutoriel utilise les commandes Azure CLI suivantes :</span><span class="sxs-lookup"><span data-stu-id="986da-109">This tutorial uses the following Azure CLI commands</span></span>

- [<span data-ttu-id="986da-110">az config param-persist delete</span><span class="sxs-lookup"><span data-stu-id="986da-110">az config param-persist delete</span></span>](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [<span data-ttu-id="986da-111">az config param-persist off</span><span class="sxs-lookup"><span data-stu-id="986da-111">az config param-persist off</span></span>](/cli/azure/config/param-persist#az_config_param_persist_off)
- [<span data-ttu-id="986da-112">az config param-persist on</span><span class="sxs-lookup"><span data-stu-id="986da-112">az config param-persist on</span></span>](/cli/azure/config/param-persist#az_config_param_persist_on)
- [<span data-ttu-id="986da-113">az config param-persist show</span><span class="sxs-lookup"><span data-stu-id="986da-113">az config param-persist show</span></span>](/cli/azure/config/param-persist#az_config_param_persist_show)
- [<span data-ttu-id="986da-114">az function app create</span><span class="sxs-lookup"><span data-stu-id="986da-114">az function app create</span></span>](/cli/azure/functionapp#az_functionapp_create)
- [<span data-ttu-id="986da-115">az group create</span><span class="sxs-lookup"><span data-stu-id="986da-115">az group create</span></span>](/cli/azure/group#az_group_create)
- [<span data-ttu-id="986da-116">az storage account create</span><span class="sxs-lookup"><span data-stu-id="986da-116">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)


<span data-ttu-id="986da-117">Si vous n’avez pas d’abonnement Azure, créez un [compte gratuit](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) avant de commencer.</span><span class="sxs-lookup"><span data-stu-id="986da-117">If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) before you begin.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="986da-118">Prérequis</span><span class="sxs-lookup"><span data-stu-id="986da-118">Prerequisites</span></span>

1. [<span data-ttu-id="986da-119">Installer l’interface de ligne de commande Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="986da-119">Install the Azure CLI</span></span>](install-azure-cli.md)

   <span data-ttu-id="986da-120">Si vous préférez, vous pouvez également utiliser Azure Cloud Shell pour effectuer les étapes décrites dans ce didacticiel.</span><span class="sxs-lookup"><span data-stu-id="986da-120">If you prefer, you can also use Azure Cloud Shell to complete the steps in this tutorial.</span></span>  <span data-ttu-id="986da-121">Azure Cloud Shell est un environnement d’interpréteur de commandes interactif que vous utilisez dans votre navigateur.</span><span class="sxs-lookup"><span data-stu-id="986da-121">Azure Cloud Shell is an interactive shell environment that you use through your browser.</span></span>  <span data-ttu-id="986da-122">Démarrez Cloud Shell à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="986da-122">Start Cloud Shell by using one of these methods:</span></span>

   - <span data-ttu-id="986da-123">Ouvrez Cloud Shell en accédant à [https://shell.azure.com](https://shell.azure.com).</span><span class="sxs-lookup"><span data-stu-id="986da-123">Open Cloud Shell by going to [https://shell.azure.com](https://shell.azure.com)</span></span>

   - <span data-ttu-id="986da-124">Sélectionnez le bouton **Cloud Shell** dans la barre de menus en haut à droite du [portail Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="986da-124">Select the **Cloud Shell** button on the menu bar at the upper right corner in the [Azure portal](https://portal.azure.com)</span></span>

1. <span data-ttu-id="986da-125">Si vous utilisez une installation locale d’Azure CLI, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="986da-125">If you are using a local install of the Azure CLI, complete the following:</span></span>
   - <span data-ttu-id="986da-126">Connectez-vous à l’aide de la commande [az login](/cli/azure/reference-index#az-login), puis suivez les étapes affichées dans votre terminal pour effectuer le processus d’authentification.</span><span class="sxs-lookup"><span data-stu-id="986da-126">Sign in using the [az login](/cli/azure/reference-index#az-login) command, then follow the steps displayed in your terminal to complete the authentication process.</span></span>

     ```azurecli
     az login
     ```
    - <span data-ttu-id="986da-127">Ce tutoriel nécessite Azure CLI version 2.12.0 ou ultérieure.</span><span class="sxs-lookup"><span data-stu-id="986da-127">This tutorial requires version 2.12.0 or later of the Azure CLI.</span></span>  <span data-ttu-id="986da-128">Exécutez [az version](/cli/azure/reference-index?#az_version) pour rechercher la version et les bibliothèques dépendantes installées.</span><span class="sxs-lookup"><span data-stu-id="986da-128">Run [az version](/cli/azure/reference-index?#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="986da-129">Pour effectuer une mise à niveau vers la dernière version, exécutez [az upgrade](/cli/azure/reference-index?#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="986da-129">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index?#az_upgrade).</span></span>

## <a name="1-determine-your-local-directory"></a><span data-ttu-id="986da-130">1. Déterminer votre répertoire local</span><span class="sxs-lookup"><span data-stu-id="986da-130">1. Determine your local directory</span></span>

<span data-ttu-id="986da-131">Les valeurs de paramètres persistants sont stockées dans le répertoire de travail du compte de stockage Azure utilisé par Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="986da-131">Persisted parameter values are stored in the working directory of the Azure storage account used by Azure Cloud Shell.</span></span>  <span data-ttu-id="986da-132">Si vous utilisez une installation locale d’Azure CLI, les valeurs sont stockées dans le répertoire de travail sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="986da-132">If you are using a local install of the Azure CLI, values are stored in the working directory on your machine.</span></span>

<span data-ttu-id="986da-133">Pour rechercher, créer ou changer le répertoire de travail utilisé par Azure CLI, utilisez ces commandes CLI bien connues.</span><span class="sxs-lookup"><span data-stu-id="986da-133">To find, create or change the working directory being used by the Azure CLI, use these familiar CLI commands.</span></span>

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a><span data-ttu-id="986da-134">2. Activer les paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-134">2. Turn on Persisted parameters</span></span>

<span data-ttu-id="986da-135">Vous devez activer les [paramètres persistants](/cli/azure/param-persist) pour pouvoir stocker les valeurs de paramètres.</span><span class="sxs-lookup"><span data-stu-id="986da-135">[Persisted parameters](/cli/azure/param-persist) must be turned on before parameter values can be stored.</span></span>  <span data-ttu-id="986da-136">Un avertissement s’affiche tant que **az config param-persist** est en phase expérimentale.</span><span class="sxs-lookup"><span data-stu-id="986da-136">You will receive a warning until **az config param-persist** moves out of the experimental stage.</span></span>  <span data-ttu-id="986da-137">Consultez [Vue d’ensemble : Types et état de référence Azure CLI](/cli/azure/reference-types-and-status) pour en savoir plus sur les types de référence, états et niveaux de prise en charge Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="986da-137">See [Overview: Azure CLI reference types and status](/cli/azure/reference-types-and-status) to learn about the Azure CLI reference types, status, and support levels.</span></span>

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a><span data-ttu-id="986da-138">3. Créer des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-138">3. Create persisted parameters</span></span>

<span data-ttu-id="986da-139">Pour stocker les valeurs de paramètres persistants, exécutez une commande Azure CLI de votre choix qui contient les paramètres à stocker.</span><span class="sxs-lookup"><span data-stu-id="986da-139">To store values for persisted parameters, execute an Azure CLI command of your choice that contains the parameters you want to store.</span></span>  <span data-ttu-id="986da-140">Par exemple, si vous créez un groupe de ressources, les paramètres **--location** et **--name** sont stockés en vue d’une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="986da-140">For example, create a resource group and the **--location** and **--name** parameters are stored for future use.</span></span>

1. <span data-ttu-id="986da-141">Stockez l’emplacement (location) et le nom du groupe de ressources (name).</span><span class="sxs-lookup"><span data-stu-id="986da-141">Store the location and resource group name.</span></span>
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. <span data-ttu-id="986da-142">À l’aide des nouveaux paramètres persistants, créez un compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="986da-142">Using the new persisted parameters, create a storage account.</span></span>

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="986da-143">Créez un paramètre persistant sans définir de nouvelle ressource.</span><span class="sxs-lookup"><span data-stu-id="986da-143">Create a persisted parameter without creating a new resource.</span></span>

   <span data-ttu-id="986da-144">Si vous ne souhaitez pas définir une nouvelle ressource Azure, les paramètres **resource_group_name** et **location** peuvent être stockés à l’aide de commandes non-create comme **show** ou **list**.</span><span class="sxs-lookup"><span data-stu-id="986da-144">If you do not want to create a new Azure resource, **resource_group_name** and **location** parameters can be stored by using non-create commands like **show** or **list**.</span></span>   <span data-ttu-id="986da-145">Pour obtenir la liste complète des paramètres pris en charge et l’action nécessaire pour conserver les valeurs, consultez [Paramètres persistants dans Azure CLI](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).</span><span class="sxs-lookup"><span data-stu-id="986da-145">See [Azure CLI persisted parameters](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) for a full list of supported parameters,   and the action needed to retain values.</span></span>  <span data-ttu-id="986da-146">Cet exemple supprime également toutes les valeurs des paramètres à l’aide de la commande [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).</span><span class="sxs-lookup"><span data-stu-id="986da-146">This example also removes all parameter values by using the [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) command.</span></span>

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the **resource_group_name** stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a><span data-ttu-id="986da-147">4. Remplacer des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-147">4. Replace persisted parameters</span></span>

<span data-ttu-id="986da-148">Pour remplacer une valeur de paramètre stockée, il suffit d’exécuter une commande contenant une valeur différente.</span><span class="sxs-lookup"><span data-stu-id="986da-148">Replacing a stored parameter value is as simple as executing a command containing a different value.</span></span>

1. <span data-ttu-id="986da-149">Définissez de nouveaux paramètres persistants.</span><span class="sxs-lookup"><span data-stu-id="986da-149">Create new persisted parameters.</span></span>
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="986da-150">Remplacez les valeurs nouvellement stockées.</span><span class="sxs-lookup"><span data-stu-id="986da-150">Replace the newly stored values.</span></span>

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > <span data-ttu-id="986da-151">Même si les paramètres persistants sont activés, vous n’êtes pas obligé de les utiliser.</span><span class="sxs-lookup"><span data-stu-id="986da-151">Even if persisted parameters are turned on, you don't have to use them.</span></span>  <span data-ttu-id="986da-152">Vous pouvez toujours exécuter des commandes en spécifiant toutes les valeurs des paramètres.</span><span class="sxs-lookup"><span data-stu-id="986da-152">You can still execute commands with all parameter values specified.</span></span>  <span data-ttu-id="986da-153">Toutefois, sachez que lorsque les paramètres persistants sont activés, _vous créez des paramètres persistants ou remplacez des paramètres persistants existants_.</span><span class="sxs-lookup"><span data-stu-id="986da-153">However, be aware that with persisted parameters turned on, _you will be creating new persisted parameters, or overwriting existing ones._</span></span>

## <a name="5-execute-sequential-commands"></a><span data-ttu-id="986da-154">5. Exécuter des commandes séquentielles</span><span class="sxs-lookup"><span data-stu-id="986da-154">5. Execute sequential commands</span></span>

<span data-ttu-id="986da-155">Ces scripts créent une application de fonction Azure à l’aide du plan Consommation.</span><span class="sxs-lookup"><span data-stu-id="986da-155">These scripts create an Azure Function app using the Consumption plan.</span></span>

### <a name="using-persisted-parameters"></a>[<span data-ttu-id="986da-156">Utilisation de paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-156">Using persisted parameters</span></span>](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[<span data-ttu-id="986da-157">Sans paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-157">Without persisted parameters</span></span>](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a><span data-ttu-id="986da-158">6. Supprimer des paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-158">6. Delete persisted parameters</span></span>

<span data-ttu-id="986da-159">Utilisez la commande [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) pour supprimer des entrées.</span><span class="sxs-lookup"><span data-stu-id="986da-159">Use the [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) command to remove entries.</span></span>

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete --name resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> <span data-ttu-id="986da-160">Les paramètres persistants ne sont pas mis à jour quand une ressource Azure est supprimée.</span><span class="sxs-lookup"><span data-stu-id="986da-160">Persisted parameters do not get updated when an Azure resource is deleted.</span></span>
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a><span data-ttu-id="986da-161">7. Désactiver les paramètres persistants</span><span class="sxs-lookup"><span data-stu-id="986da-161">7. Turn persisted parameters off</span></span>

<span data-ttu-id="986da-162">Vous pouvez désactiver les paramètres persistants à l’aide de la commande [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), mais les données enregistrées des paramètres persistants ne sont pas supprimées.</span><span class="sxs-lookup"><span data-stu-id="986da-162">You can turn persisted parameters off by using the [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) command, but your saved persisted parameters data won't be deleted.</span></span>

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a><span data-ttu-id="986da-163">8. Nettoyer les ressources</span><span class="sxs-lookup"><span data-stu-id="986da-163">8. Clean up resources</span></span>

<span data-ttu-id="986da-164">Quand vous n’avez plus besoin du groupe de ressources, utilisez la commande [az group delete](/cli/azure/group) pour supprimer celui-ci ainsi que toutes les ressources associées.</span><span class="sxs-lookup"><span data-stu-id="986da-164">When no longer needed, use the [az group delete](/cli/azure/group) command to remove the resource group, and all related resources.</span></span>

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a><span data-ttu-id="986da-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="986da-165">See also</span></span>

- [<span data-ttu-id="986da-166">Comment utiliser des paramètres persistants Azure CLI</span><span class="sxs-lookup"><span data-stu-id="986da-166">(How to work with Azure CLI persisted parameters</span></span>](param-persist-howto.md)
- [<span data-ttu-id="986da-167">Configuration d’Azure CLI avec az configure</span><span class="sxs-lookup"><span data-stu-id="986da-167">Azure CLI Configuration using az configure</span></span>](/cli/azure/azure-cli-configuration)
