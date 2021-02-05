---
title: Gérer les groupes de ressources Azure avec Azure CLI
description: Découvrez les groupes de ressources Azure et l’utilisation d’Azure CLI pour gérer vos groupes de ressources. Découvrez les groupes de ressources persistants et par défaut.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496076"
---
# <a name="working-with-resource-groups-in-azure-cli"></a><span data-ttu-id="f1a62-104">Utilisation de groupes de ressources dans Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f1a62-104">Working with resource groups in Azure CLI</span></span>

<span data-ttu-id="f1a62-105">Un groupe de ressources Azure est un conteneur réunissant les ressources associées d’une solution Azure.</span><span class="sxs-lookup"><span data-stu-id="f1a62-105">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="f1a62-106">Un groupe de ressources peut contenir du stockage, des machines virtuelles, des applications, des tableaux de bord, des services, soit presque tout ce à quoi vous avez affaire dans Azure.</span><span class="sxs-lookup"><span data-stu-id="f1a62-106">A resource group might contain storage, virtual machines, apps, dashboards, services, or almost anything you deal with in Azure.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="f1a62-107">Créer un groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="f1a62-107">Create a resource group</span></span>

<span data-ttu-id="f1a62-108">Pour créer un groupe de ressources, utilisez la commande [az group create](/cli/azure/group#az_group_create) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-108">To create a resource group, use the [az group create](/cli/azure/group#az_group_create) command:</span></span>

```azurecli
az group create --name MyResourceGroup --location eastus
```

<span data-ttu-id="f1a62-109">Un groupe de ressources appartient à un seul emplacement.</span><span class="sxs-lookup"><span data-stu-id="f1a62-109">A resource group belongs to a single location.</span></span> <span data-ttu-id="f1a62-110">Pour voir tous les emplacements pris en charge dans votre abonnement actuel, exécutez la commande [az account list-locations](/cli/azure/account#az_account_list_locations) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-110">To see all the locations supported in your current subscription, run the [az account list-locations](/cli/azure/account#az_account_list_locations) command:</span></span>

```azurecli
az account list-locations
```

<span data-ttu-id="f1a62-111">Pour voir tous les groupes de ressources de votre abonnement actuel, utilisez la commande [az group list](/cli/azure/group#az_group_list) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-111">To see all the resource groups for your current subscription, use the [az group list](/cli/azure/group#az_group_list) command:</span></span>

```azurecli
az group list --output table
```

> [!TIP]
> <span data-ttu-id="f1a62-112">Le paramètre `--output` est un paramètre global, disponible pour toutes les commandes.</span><span class="sxs-lookup"><span data-stu-id="f1a62-112">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="f1a62-113">La valeur **table** présente la sortie dans un format convivial.</span><span class="sxs-lookup"><span data-stu-id="f1a62-113">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="f1a62-114">Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="f1a62-114">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="f1a62-115">Quand vous créez une ressource, vous la créez dans un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="f1a62-115">When you create a resource, you create it in a resource group.</span></span> <span data-ttu-id="f1a62-116">L’exemple suivant montre un compte de stockage créé à l’aide de la commande [az storage account create](/cli/azure/storage/account#az_storage_account_create) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-116">The following example shows a storage account created by using the [az storage account create](/cli/azure/storage/account#az_storage_account_create) command:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

<span data-ttu-id="f1a62-117">Pour supprimer un groupe de ressources, exécutez la commande [az group delete](/cli/azure/group#az_group_delete) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-117">To remove a resource group, run the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
```

<span data-ttu-id="f1a62-118">Quand vous supprimez un groupe de ressources, vous supprimez toutes les ressources qui lui appartiennent.</span><span class="sxs-lookup"><span data-stu-id="f1a62-118">When you remove a resource group, you delete all the resources that belong to it.</span></span> <span data-ttu-id="f1a62-119">Aucune option ne permet d’annuler la suppression des ressources.</span><span class="sxs-lookup"><span data-stu-id="f1a62-119">There's no option to undelete resources.</span></span> <span data-ttu-id="f1a62-120">Si vous essayez l’une des commandes mentionnées dans cet article, la suppression des groupes de ressources que vous créez nettoie votre compte.</span><span class="sxs-lookup"><span data-stu-id="f1a62-120">If you try any of the commands in this article, deleting the resource groups you create cleans up your account.</span></span>

## <a name="persist-a-resource-group"></a><span data-ttu-id="f1a62-121">Rendre persistant un groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="f1a62-121">Persist a resource group</span></span>

<span data-ttu-id="f1a62-122">La persistance des paramètres vous permet de réutiliser des valeurs pour certains paramètres, notamment des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="f1a62-122">Parameter persistence allows you to reuse values for certain parameters, including resource groups.</span></span>

<span data-ttu-id="f1a62-123">Tout d’abord, activez la fonctionnalité de persistance à l’aide de la commande [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-123">First, turn on the persistence feature by using the [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) command:</span></span>

```azurecli
az config param-persist on
```

<span data-ttu-id="f1a62-124">Une fois la persistance activée, créez un autre groupe de ressources :</span><span class="sxs-lookup"><span data-stu-id="f1a62-124">After turning on persistence, create another resource group:</span></span>

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

<span data-ttu-id="f1a62-125">Tant que la persistance est activée, vous pouvez laisser le paramètre `--resource-group` hors des commandes ultérieures.</span><span class="sxs-lookup"><span data-stu-id="f1a62-125">As long as persistence is on, your can leave the `--resource-group` parameter out of future commands.</span></span> <span data-ttu-id="f1a62-126">La commande suivante crée un compte de stockage dans le groupe **OtherResourceGroup** :</span><span class="sxs-lookup"><span data-stu-id="f1a62-126">The following command creates a storage account in the **OtherResourceGroup** group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="f1a62-127">Si vous spécifiez un groupe de ressources dans la commande, il est prioritaire.</span><span class="sxs-lookup"><span data-stu-id="f1a62-127">If you specify a resource group in the command, that takes precedence.</span></span> <span data-ttu-id="f1a62-128">La commande suivante crée un groupe de stockage dans un groupe de ressources appelé **StorageGroups** :</span><span class="sxs-lookup"><span data-stu-id="f1a62-128">The following command creates a storage group in a resource group called **StorageGroups**:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

<span data-ttu-id="f1a62-129">En revanche, une fois que vous spécifiez un autre groupe de ressources en tant que valeur, Azure CLI redéfinit la valeur rendue persistante.</span><span class="sxs-lookup"><span data-stu-id="f1a62-129">Once you specify another resource group as a value, however, Azure CLI resets the persisted value.</span></span> <span data-ttu-id="f1a62-130">Les nouvelles commandes utilisent **StorageGroups** en tant que groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="f1a62-130">New commands use **StorageGroups** as the resource group.</span></span> <span data-ttu-id="f1a62-131">Vous pouvez afficher les valeurs rendues persistantes à l’aide de la commande [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-131">You can see the persisted values by using the [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) command:</span></span>

```azurecli
az config param-persist show
```

<span data-ttu-id="f1a62-132">Cette commande vous montre les valeurs actuellement rendues persistantes.</span><span class="sxs-lookup"><span data-stu-id="f1a62-132">This command shows you the current persisted values.</span></span> <span data-ttu-id="f1a62-133">Ces valeurs sont stockées dans un fichier appelé *local_context_\<username>* dans un répertoire masqué appelé *.azure*.</span><span class="sxs-lookup"><span data-stu-id="f1a62-133">These values are stored in a file called *local_context_\<username>* in a hidden directory called *.azure*.</span></span> <span data-ttu-id="f1a62-134">Azure CLI crée le répertoire à votre emplacement actuel quand vous créez une première valeur persistante.</span><span class="sxs-lookup"><span data-stu-id="f1a62-134">Azure CLI creates the directory in your current location when you first create a persistent value.</span></span>

<span data-ttu-id="f1a62-135">Quand vous avez terminé d’utiliser des paramètres persistants, exécutez la commande [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-135">When you're done using persisted parameters, run the [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) command:</span></span>

```azurecli
az config param-persist off
```

<span data-ttu-id="f1a62-136">Azure CLI enregistre vos valeurs persistantes.</span><span class="sxs-lookup"><span data-stu-id="f1a62-136">Azure CLI saves your persisted values.</span></span> <span data-ttu-id="f1a62-137">Vous pouvez les voir dans le fichier de contexte local.</span><span class="sxs-lookup"><span data-stu-id="f1a62-137">You can see them in the local context file.</span></span> <span data-ttu-id="f1a62-138">Si vous réactivez la persistance des paramètres, ces valeurs sont déjà définies.</span><span class="sxs-lookup"><span data-stu-id="f1a62-138">If you turn on parameter persistence again, those values are already set.</span></span>

<span data-ttu-id="f1a62-139">Pour plus d’informations sur l’utilisation des commandes [az config param-persist](/cli/azure/config/param-persist), consultez [Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles](/cli/azure/param-persist-tutorial).</span><span class="sxs-lookup"><span data-stu-id="f1a62-139">For more information about using the [az config param-persist](/cli/azure/config/param-persist) commands, see [Use persisted parameters to simplify sequential Azure CLI commands](/cli/azure/param-persist-tutorial).</span></span>

## <a name="set-a-default-resource-group"></a><span data-ttu-id="f1a62-140">Définir un groupe de ressources par défaut</span><span class="sxs-lookup"><span data-stu-id="f1a62-140">Set a default resource group</span></span>

<span data-ttu-id="f1a62-141">Vous pouvez définir un groupe de ressources par défaut pour toutes les commandes que vous exécutez à partir de votre Azure CLI local ou d’Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f1a62-141">You can set a default resource group for all the commands that you run from your local Azure CLI or from Azure Cloud Shell.</span></span> <span data-ttu-id="f1a62-142">Azure CLI stocke cette configuration localement dans un fichier *config*.</span><span class="sxs-lookup"><span data-stu-id="f1a62-142">Azure CLI stores this configuration locally in a *config* file.</span></span> <span data-ttu-id="f1a62-143">Pour afficher votre configuration actuelle, exécutez la commande [az config get](/cli/azure/config#az_config_get) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-143">To see your current configuration, run the [az config get](/cli/azure/config#az_config_get) command:</span></span>

```azurecli
az config get
```

<span data-ttu-id="f1a62-144">Le résultat présente les groupes de ressources par défaut et d’autres valeurs par défaut.</span><span class="sxs-lookup"><span data-stu-id="f1a62-144">The result shows default resource groups and other default values.</span></span> <span data-ttu-id="f1a62-145">Si vous utilisez Azure CLI pour la première fois, les résultats risquent d’être vides.</span><span class="sxs-lookup"><span data-stu-id="f1a62-145">If you're using Azure CLI for the first time, the results might be empty.</span></span>

<span data-ttu-id="f1a62-146">Pour définir un groupe de ressources par défaut pour votre installation Azure CLI, exécutez la commande [az config set](/cli/azure/config#az_config_set) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-146">To set a default resource group for your Azure CLI installation, run the [az config set](/cli/azure/config#az_config_set) command:</span></span>

```azurecli
az config set defaults.group=MyResourceGroup
```

<span data-ttu-id="f1a62-147">La commande définit une valeur pour une clé spécifiée, dans cet exemple `defaults.group`.</span><span class="sxs-lookup"><span data-stu-id="f1a62-147">The command sets a value for a specified key, in this case `defaults.group`.</span></span> <span data-ttu-id="f1a62-148">Pour connaître les options de configuration disponibles, consultez [Configuration d’Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="f1a62-148">For available configuration options, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

> [!NOTE]
> <span data-ttu-id="f1a62-149">La commande [az config set](/cli/azure/config#az_config_set) ne valide pas l’existence du groupe de ressources que vous entrez.</span><span class="sxs-lookup"><span data-stu-id="f1a62-149">The [az config set](/cli/azure/config#az_config_set) command does not validate the existence of the resource group you enter.</span></span> <span data-ttu-id="f1a62-150">La commande stocke simplement la paire clé-valeur.</span><span class="sxs-lookup"><span data-stu-id="f1a62-150">The command simply stores the key-value pair.</span></span>

<span data-ttu-id="f1a62-151">Une fois que vous avez exécuté la commande, les deux commandes suivantes donnent le même résultat :</span><span class="sxs-lookup"><span data-stu-id="f1a62-151">After you run the command, the following two commands would give you the same result:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

<span data-ttu-id="f1a62-152">Un groupe de ressources appartient à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="f1a62-152">A resource group belongs to a subscription.</span></span> <span data-ttu-id="f1a62-153">Si votre organisation a plusieurs abonnements, vous devez définir l’abonnement d’un groupe de ressources avant de l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="f1a62-153">If your organization has more than one subscription, you need to set that subscription before working with a resource group in the subscription.</span></span> <span data-ttu-id="f1a62-154">Si la valeur par défaut d’un groupe de ressources ne correspond pas à votre abonnement actuel, une erreur se produit.</span><span class="sxs-lookup"><span data-stu-id="f1a62-154">If the default value of a resource group does not belong to your current subscription, an error results.</span></span> <span data-ttu-id="f1a62-155">Pour plus d’informations sur les abonnements multiples, consultez [Utiliser plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f1a62-155">For more information about multiple subscriptions, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="f1a62-156">Vous n’avez pas besoin de réinitialiser la valeur par défaut pour utiliser d’autres groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="f1a62-156">You don't have to reset the default to use other resource groups.</span></span> <span data-ttu-id="f1a62-157">Il vous suffit plutôt de spécifier le groupe de ressources :</span><span class="sxs-lookup"><span data-stu-id="f1a62-157">Instead, specify the resource group:</span></span>

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

<span data-ttu-id="f1a62-158">La valeur par défaut est pour vous seulement.</span><span class="sxs-lookup"><span data-stu-id="f1a62-158">The default value is for you only.</span></span> <span data-ttu-id="f1a62-159">Elle n’affecte pas les autres utilisateurs ni les modifications que vous apportez par le biais du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="f1a62-159">It won't affect other users or changes you make through the Azure portal.</span></span>

<span data-ttu-id="f1a62-160">Si vous utilisez des valeurs de paramètre persistantes, comme décrit dans cet article, ces valeurs sont prioritaires par rapport aux valeurs par défaut définies dans le fichier *config*.</span><span class="sxs-lookup"><span data-stu-id="f1a62-160">If you are using persisted parameter values, as described in this article, those values take precedence over defaults set in the *config* file.</span></span>

## <a name="clean-up-resources"></a><span data-ttu-id="f1a62-161">Nettoyer les ressources</span><span class="sxs-lookup"><span data-stu-id="f1a62-161">Clean up resources</span></span>

<span data-ttu-id="f1a62-162">Si vous avez essayé l’une des commandes mentionnées dans cet article, vous pouvez supprimer toutes les ressources que vous avez créées en utilisant la commande [az group delete](/cli/azure/group#az_group_delete) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-162">If you tried any of the commands in this article, you can remove any resources you created by using the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

<span data-ttu-id="f1a62-163">Cette commande supprime le groupe et toutes les ressources qu’il contient en une seule opération.</span><span class="sxs-lookup"><span data-stu-id="f1a62-163">This command removes the group and all the resources that it contains at once.</span></span>

<span data-ttu-id="f1a62-164">Vous pouvez supprimer les paramètres persistants en exécutant la commande [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) :</span><span class="sxs-lookup"><span data-stu-id="f1a62-164">You can remove the persistent parameters by running the [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) command:</span></span>

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a><span data-ttu-id="f1a62-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1a62-165">See also</span></span>

[<span data-ttu-id="f1a62-166">Configuration d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f1a62-166">Azure CLI configuration</span></span>](/cli/azure/azure-cli-configuration)

[<span data-ttu-id="f1a62-167">Tutoriel : Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles</span><span class="sxs-lookup"><span data-stu-id="f1a62-167">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>](/cli/azure/param-persist-tutorial)

[<span data-ttu-id="f1a62-168">Utilisez plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="f1a62-168">Use multiple Azure subscriptions</span></span>](manage-azure-subscriptions-azure-cli.md)
