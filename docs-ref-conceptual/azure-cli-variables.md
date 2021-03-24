---
title: Spécification de valeurs dans les commandes Azure CLI
description: Découvrez comment passer des valeurs aux commandes Azure CLI, notamment des variables, et comment réutiliser des valeurs courantes.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-cli
ms.topic: how-to
ms.date: 03/01/2021
ms.custom: template-how-to
ms.openlocfilehash: 18bd938403d18a14278a7b8a97ca93bc0e0d0f1c
ms.sourcegitcommit: f9e23f29c59c6957d3df4d5ca2f4425093e6fd80
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/16/2021
ms.locfileid: "103554912"
---
# <a name="specifying-values-in-azure-cli-commands"></a><span data-ttu-id="dc704-103">Spécification de valeurs dans les commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dc704-103">Specifying values in Azure CLI commands</span></span>

<span data-ttu-id="dc704-104">En plus de spécifier des valeurs directement dans une commande, vous pouvez recourir à diverses méthodes pour fournir des valeurs :</span><span class="sxs-lookup"><span data-stu-id="dc704-104">In addition to specifying values directly in a command, you can provide values in several ways:</span></span>

* <span data-ttu-id="dc704-105">Utiliser des variables shell</span><span class="sxs-lookup"><span data-stu-id="dc704-105">Use shell variables</span></span>
* <span data-ttu-id="dc704-106">Définir un abonnement à utiliser dans plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="dc704-106">Set a subscription for use in multiple commands</span></span>
* <span data-ttu-id="dc704-107">Créer des valeurs par défaut pour certains paramètres</span><span class="sxs-lookup"><span data-stu-id="dc704-107">Create default values for some parameters</span></span>
* <span data-ttu-id="dc704-108">Utiliser des valeurs persistantes pour certains paramètres</span><span class="sxs-lookup"><span data-stu-id="dc704-108">Use persistent values for some parameters</span></span>

<span data-ttu-id="dc704-109">Cet article décrit différentes façons de spécifier des valeurs dans les commandes Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="dc704-109">This article discusses various ways to specify values in Azure CLI commands.</span></span>

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="use-shell-variables"></a><span data-ttu-id="dc704-110">Utiliser des variables shell</span><span class="sxs-lookup"><span data-stu-id="dc704-110">Use shell variables</span></span>

<span data-ttu-id="dc704-111">Azure CLI s’exécute dans un interpréteur de commandes (shell).</span><span class="sxs-lookup"><span data-stu-id="dc704-111">Azure CLI runs in a shell.</span></span> <span data-ttu-id="dc704-112">Cet article utilise Bash.</span><span class="sxs-lookup"><span data-stu-id="dc704-112">This article uses Bash.</span></span> <span data-ttu-id="dc704-113">Pour plus d’informations sur les autres shells, consultez [Utiliser Azure CLI efficacement](/cli/azure/use-cli-effectively).</span><span class="sxs-lookup"><span data-stu-id="dc704-113">For information about other shells, see [Use Azure CLI effectively](/cli/azure/use-cli-effectively).</span></span> <span data-ttu-id="dc704-114">Vous pouvez utiliser des variables dans Bash pour passer des valeurs de paramètres à des commandes.</span><span class="sxs-lookup"><span data-stu-id="dc704-114">You can use variables in Bash to pass values for parameters to commands.</span></span> <span data-ttu-id="dc704-115">Les variables permettent également de réutiliser des commandes (fragmentaires ou dans des scripts).</span><span class="sxs-lookup"><span data-stu-id="dc704-115">Using variables also allows reuse of commands, either piecemeal or in scripts.</span></span>

<span data-ttu-id="dc704-116">Cet exemple crée un disque de stockage du même type que celui d’une machine virtuelle existante.</span><span class="sxs-lookup"><span data-stu-id="dc704-116">This example creates a new storage disk of the same type as the storage disk on an existing virtual machine.</span></span>

```azurecli
# Assign values to variables
MyResourceGroup=ContosoRGforVM
MySubscription="Contoso subscription"
vmName=VM01

# Get a value for a variable based on an existing virtual machine
osType=$(az vm get-instance-view --resource-group $MyResourceGroup \
   --name $vmName --subscription "$MySubscription" \
   --query 'storageProfile.osDisk.osType' --output tsv)

# Create a disk of the same type by using the variable value
az disk create --resource-group $MyResourceGroup --name DestinationDisk --size-gb 20 --os-type $osType
```

<span data-ttu-id="dc704-117">Cet exemple affecte des valeurs à des variables qui sont réutilisées, comme **MyResourceGroup**.</span><span class="sxs-lookup"><span data-stu-id="dc704-117">This example assigns values to variables that are reused, like **MyResourceGroup**.</span></span> <span data-ttu-id="dc704-118">Une commande obtient une valeur à affecter à **osType**.</span><span class="sxs-lookup"><span data-stu-id="dc704-118">A command gets a value to assign to **osType**.</span></span>

<span data-ttu-id="dc704-119">Quand vous affectez une valeur à une variable à partir d’une autre commande, vérifiez que la commande utilise un format de sortie compatible.</span><span class="sxs-lookup"><span data-stu-id="dc704-119">When you assign a value to a variable from another command, be sure that the command uses a compatible output format.</span></span> <span data-ttu-id="dc704-120">La commande [az vm get-instance-view](/cli/azure/vm#az_vm_get_instance_view) utilise le format de sortie `tsv`.</span><span class="sxs-lookup"><span data-stu-id="dc704-120">The [az vm get-instance-view](/cli/azure/vm#az_vm_get_instance_view) command uses the `tsv` output format.</span></span> <span data-ttu-id="dc704-121">Cette option retourne des valeurs sans mise en forme, clé ou autre symbole supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="dc704-121">This option returns values without extra formatting, keys, or other symbols.</span></span> <span data-ttu-id="dc704-122">Certains formats de sortie incluent des structures ou des caractères comme des guillemets.</span><span class="sxs-lookup"><span data-stu-id="dc704-122">Some output formats include structure or characters like quotation marks.</span></span> <span data-ttu-id="dc704-123">Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="dc704-123">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="dc704-124">Dans cet exemple, la variable **MySubscription** doit être entre guillemets.</span><span class="sxs-lookup"><span data-stu-id="dc704-124">In this example, the **MySubscription** variable must be in quotation marks.</span></span> <span data-ttu-id="dc704-125">Sa valeur contient des espaces que la commande ne peut pas analyser.</span><span class="sxs-lookup"><span data-stu-id="dc704-125">Its value contains spaces, which the command can't parse.</span></span> <span data-ttu-id="dc704-126">Si vous travaillez uniquement avec des ID d’abonnement, vous n’avez pas besoin d’utiliser des guillemets.</span><span class="sxs-lookup"><span data-stu-id="dc704-126">If you work only with subscription IDs, you don't need to use quotation marks.</span></span>

## <a name="set-a-subscription"></a><span data-ttu-id="dc704-127">Définir un abonnement</span><span class="sxs-lookup"><span data-stu-id="dc704-127">Set a subscription</span></span>

<span data-ttu-id="dc704-128">De nombreuses commandes nécessitent un abonnement spécifique.</span><span class="sxs-lookup"><span data-stu-id="dc704-128">Many commands require a specific subscription.</span></span> <span data-ttu-id="dc704-129">Les ressources Azure existent dans des groupes de ressources, lesquels existent dans des abonnements.</span><span class="sxs-lookup"><span data-stu-id="dc704-129">Azure resources exist in resource groups, which exist in subscriptions.</span></span> <span data-ttu-id="dc704-130">Azure CLI utilise un abonnement par défaut quand vous êtes dans une session.</span><span class="sxs-lookup"><span data-stu-id="dc704-130">Azure CLI uses a default subscription when you are in a session.</span></span> <span data-ttu-id="dc704-131">Pour voir la valeur de votre abonnement actif, exécutez la commande [az account show](/cli/azure/account#az_account_show) :</span><span class="sxs-lookup"><span data-stu-id="dc704-131">To see your current subscription value, run the [az account show](/cli/azure/account#az_account_show) command:</span></span>

```azurecli
az account show --output table
```

<span data-ttu-id="dc704-132">Il est possible que vous n’ayez accès qu’à un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="dc704-132">You might have access to only one subscription.</span></span> <span data-ttu-id="dc704-133">Pour plus d’informations, consultez [Utiliser des abonnements Azure avec Azure CLI](/cli/azure/manage-azure-subscriptions-azure-cli). Vous pouvez utiliser la commande [az account set](/cli/azure/account#az-account-set) pour définir votre abonnement actif :</span><span class="sxs-lookup"><span data-stu-id="dc704-133">For more information, see [Use Azure subscriptions with Azure CLI](/cli/azure/manage-azure-subscriptions-azure-cli) You can use the [az account set](/cli/azure/account#az-account-set) command to set your current subscription:</span></span>

```azurecli
az account set --subscription "My Demos"
```

<span data-ttu-id="dc704-134">Après avoir défini votre abonnement, vous pouvez omettre le paramètre `--Subscription`.</span><span class="sxs-lookup"><span data-stu-id="dc704-134">After you set your subscription, you can omit `--Subscription` parameter.</span></span> <span data-ttu-id="dc704-135">Pour plus d’informations, consultez [Utiliser des abonnements Azure avec Azure CLI](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="dc704-135">For more information, see [Use Azure subscriptions with Azure CLI](manage-azure-subscriptions-azure-cli.md).</span></span>

## <a name="create-default-values"></a><span data-ttu-id="dc704-136">Créer des valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="dc704-136">Create default values</span></span>

<span data-ttu-id="dc704-137">Vous pouvez définir des valeurs pour certains paramètres en utilisant la commande [az config set](/cli/azure/config#az_config_set).</span><span class="sxs-lookup"><span data-stu-id="dc704-137">You can set values for some parameters by using the [az config set](/cli/azure/config#az_config_set) command.</span></span> <span data-ttu-id="dc704-138">Cet exemple définit un groupe de ressources par défaut :</span><span class="sxs-lookup"><span data-stu-id="dc704-138">This example sets a default resource group:</span></span>

```azurecli
az config set defaults.group=ContosoRGforVM
```

<span data-ttu-id="dc704-139">Après avoir exécuté cette commande, exécutez celle-ci pour créer un compte de stockage dans le groupe de ressources ContosoRGforVM :</span><span class="sxs-lookup"><span data-stu-id="dc704-139">After running this command, you can run the following command to create a storage account in the ContosoRGforVM resource group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="dc704-140">Notez qu’aucun groupe de ressources n’est spécifié dans la commande.</span><span class="sxs-lookup"><span data-stu-id="dc704-140">Notice that there's no resource group specified in the command.</span></span> <span data-ttu-id="dc704-141">Pour plus d’informations, consultez [Définir un groupe de ressources par défaut](manage-azure-groups-azure-cli.md#set-a-default-resource-group).</span><span class="sxs-lookup"><span data-stu-id="dc704-141">For more information, see [Set a default resource group](manage-azure-groups-azure-cli.md#set-a-default-resource-group).</span></span>

> [!TIP]
> <span data-ttu-id="dc704-142">Les commandes qui obtiennent les valeurs de paramètres de différentes manières peuvent prêter à confusion.</span><span class="sxs-lookup"><span data-stu-id="dc704-142">Commands getting values for parameters in different ways can be confusing.</span></span> <span data-ttu-id="dc704-143">Si une commande donne un résultat inattendu, comme l’impossibilité de trouver un groupe de ressources, il peut y avoir une valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="dc704-143">If a command gives an unexpected result, such as not being able to find a resource group, there may be a default value.</span></span>
>
> <span data-ttu-id="dc704-144">Si vous rencontrez une erreur, réexécutez la commande avec le paramètre et la valeur spécifiés.</span><span class="sxs-lookup"><span data-stu-id="dc704-144">If you encounter an error, run the command again with the parameter and value specified.</span></span> <span data-ttu-id="dc704-145">Une valeur explicite pour un paramètre est toujours prioritaire sur les autres options.</span><span class="sxs-lookup"><span data-stu-id="dc704-145">An explicit value for a parameter always takes precedence over other options.</span></span>

<span data-ttu-id="dc704-146">Vous pouvez spécifier des valeurs pour plusieurs paramètres de cette façon.</span><span class="sxs-lookup"><span data-stu-id="dc704-146">You can specify values for several parameters this way.</span></span> <span data-ttu-id="dc704-147">Pour plus d’informations, consultez [Configuration d’Azure CLI](azure-cli-configuration.md).</span><span class="sxs-lookup"><span data-stu-id="dc704-147">For more information, see [Azure CLI configuration](azure-cli-configuration.md).</span></span>

## <a name="use-persistent-values"></a><span data-ttu-id="dc704-148">Utiliser des valeurs persistantes</span><span class="sxs-lookup"><span data-stu-id="dc704-148">Use persistent values</span></span>

<span data-ttu-id="dc704-149">Les valeurs persistantes vous permettent de spécifier une valeur de paramètre une seule fois.</span><span class="sxs-lookup"><span data-stu-id="dc704-149">Persisted parameter values allow you to specify a value only once.</span></span> <span data-ttu-id="dc704-150">Si vous effectuez plusieurs actions associées dans un groupe de ressources, vous n’êtes pas obligé de spécifier ce groupe à plusieurs reprises.</span><span class="sxs-lookup"><span data-stu-id="dc704-150">If you're doing several related actions in a resource group, you don't have to specify that group repeatedly.</span></span>

<span data-ttu-id="dc704-151">Exécutez cette commande pour rendre une valeur de paramètre persistante :</span><span class="sxs-lookup"><span data-stu-id="dc704-151">Run this command to persist a parameter value:</span></span>

```azurecli
az config param-persist on
```

<span data-ttu-id="dc704-152">Une fois la persistance activée, créez un groupe de ressources :</span><span class="sxs-lookup"><span data-stu-id="dc704-152">After turning on persistence, create a resource group:</span></span>

 ```azurecli
az group create --name ContosoStorageRG --location eastus
```

<span data-ttu-id="dc704-153">Tant que la persistance est activée, vous pouvez laisser le paramètre `--resource-group` hors des commandes ultérieures.</span><span class="sxs-lookup"><span data-stu-id="dc704-153">As long as persistence is on, your can leave the `--resource-group` parameter out of future commands.</span></span> <span data-ttu-id="dc704-154">La commande suivante crée un compte de stockage dans le groupe de ressources ContosoStorageRG :</span><span class="sxs-lookup"><span data-stu-id="dc704-154">The following command creates a storage account in the ContosoStorageRG resource group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="dc704-155">Pour plus d’informations, consultez [Paramètre persistant Azure CLI](/cli/azure/param-persist-howto).</span><span class="sxs-lookup"><span data-stu-id="dc704-155">For more information, see [Azure CLI persisted parameter](/cli/azure/param-persist-howto).</span></span>

## <a name="clean-up-resources"></a><span data-ttu-id="dc704-156">Nettoyer les ressources</span><span class="sxs-lookup"><span data-stu-id="dc704-156">Clean up resources</span></span>

<span data-ttu-id="dc704-157">Si vous avez créé des ressources pour essayer l’une des commandes de cet article, vous pouvez les supprimer en utilisant la commande [az group delete](/cli/azure/group#az_group_delete) :</span><span class="sxs-lookup"><span data-stu-id="dc704-157">If you created resources to try any of the commands in this article, you can remove them by using the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name ContosoRGforVM
az group delete --name ContosoStorageRG
```

<span data-ttu-id="dc704-158">Cette commande supprime le groupe et toutes les ressources qu’il contient en une seule opération.</span><span class="sxs-lookup"><span data-stu-id="dc704-158">This command removes the group and all the resources that it contains at once.</span></span>

<span data-ttu-id="dc704-159">Vous pouvez supprimer les paramètres persistants en exécutant la commande [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) :</span><span class="sxs-lookup"><span data-stu-id="dc704-159">You can remove the persistent parameters by running the [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) command:</span></span>

```azurecli
az config param-persist delete --all
```

## <a name="next-steps"></a><span data-ttu-id="dc704-160">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="dc704-160">Next steps</span></span>

* [<span data-ttu-id="dc704-161">Paramètre persistant Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dc704-161">Azure CLI persisted parameter</span></span>](param-persist-howto.md)
* [<span data-ttu-id="dc704-162">Utilisation de groupes de ressources dans Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dc704-162">Working with resource groups in Azure CLI</span></span>](manage-azure-groups-azure-cli.md)
* [<span data-ttu-id="dc704-163">Créer une demande de support Azure dans Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dc704-163">Create an Azure support request in Azure CLI</span></span>](azure-cli-support-request.md)