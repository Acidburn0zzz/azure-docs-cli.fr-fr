---
title: "Bien démarrer avec Azure CLI 2.0"
description: "Bien démarrer avec Azure CLI 2.0 sur Linux, Mac ou Windows."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 689b8f4d77af5a6f398c0dd85e922baa398f767a
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/26/2018
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="7af80-104">Bien démarrer avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="7af80-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="7af80-105">Azure CLI 2.0 est la nouvelle expérience de ligne de commande Azure pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-105">The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.</span></span>
<span data-ttu-id="7af80-106">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou [l’installer](install-azure-cli.md) sur macOS, Linux et Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="7af80-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="7af80-107">Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="7af80-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span>
<span data-ttu-id="7af80-108">Cet article vous aide à bien démarrer et explique les concepts de base.</span><span class="sxs-lookup"><span data-stu-id="7af80-108">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

<span data-ttu-id="7af80-109">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7af80-109">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

## <a name="connect"></a><span data-ttu-id="7af80-110">Connecter</span><span class="sxs-lookup"><span data-stu-id="7af80-110">Connect</span></span>

<span data-ttu-id="7af80-111">La façon la plus simple de commencer est de [lancer Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="7af80-111">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="7af80-112">Lancez Cloud Shell dans le volet de navigation supérieur du Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-112">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Icône Shell](media/get-started-with-azure-cli/shell-icon.png)

2. <span data-ttu-id="7af80-114">Sélectionnez l’abonnement que vous souhaitez utiliser, et créez un compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="7af80-114">Choose the subscription you want to use and create a storage account.</span></span>

   ![Créez un compte de stockage.](media/get-started-with-azure-cli/storage-prompt.png)

<span data-ttu-id="7af80-116">Vous pouvez également [installer](install-azure-cli.md) l’interface de ligne de commande et l’exécuter localement à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="7af80-116">You can also [install](install-azure-cli.md) the CLI and run it locally from the command line.</span></span> <span data-ttu-id="7af80-117">Après avoir installé l’interface CLI, exécutez `az login` pour vous connecter avec votre abonnement par défaut.</span><span class="sxs-lookup"><span data-stu-id="7af80-117">Once you have installed the CLI, run `az login` to log in with your default subscription.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="7af80-118">Création d’un groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="7af80-118">Create a Resource Group</span></span>

<span data-ttu-id="7af80-119">Maintenant que tout est configuré, nous allons utiliser Azure CLI pour créer des ressources dans Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-119">Now that we've got everything set up, let's use the Azure CLI to create resources within Azure.</span></span>

<span data-ttu-id="7af80-120">Nous devons d’abord créer un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="7af80-120">First, create a Resource Group.</span></span>  <span data-ttu-id="7af80-121">Les groupes de ressources dans Azure permettent de gérer plusieurs ressources à regrouper logiquement.</span><span class="sxs-lookup"><span data-stu-id="7af80-121">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group.</span></span>  <span data-ttu-id="7af80-122">Par exemple, vous pouvez créer un groupe de ressources pour une application ou un projet, et y ajouter une machine virtuelle, une base de données et un service CDN.</span><span class="sxs-lookup"><span data-stu-id="7af80-122">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="7af80-123">Nous allons créer un groupe de ressources nommé « MyResourceGroup » dans la région *westus2* d’Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-123">Let's create a resource group named "MyResourceGroup" in the *westus2* region of Azure.</span></span>  <span data-ttu-id="7af80-124">Pour ce faire, tapez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="7af80-124">To do so type the following command:</span></span>

```azurecli-interactive
az group create -n MyResourceGroup -l westus2
```

<span data-ttu-id="7af80-125">Une fois le groupe de ressources créé, la commande `az group create` génère plusieurs propriétés de la ressource nouvellement créée :</span><span class="sxs-lookup"><span data-stu-id="7af80-125">Once the resource group has been created, the `az group create` command outputs several properties of the newly created resource:</span></span>

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="7af80-126">Créer une machine virtuelle Linux</span><span class="sxs-lookup"><span data-stu-id="7af80-126">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="7af80-127">Maintenant que nous avons notre groupe de ressources, nous allons y créer une machine virtuelle Linux.</span><span class="sxs-lookup"><span data-stu-id="7af80-127">Now that we have our resource group, let's create a Linux VM within it.</span></span>

<span data-ttu-id="7af80-128">Vous pouvez créer une machine virtuelle Linux à l’aide de l’image UbuntuTLS populaire, avec deux disques de stockage liés de 10 Go et 20 Go, à l’aide de la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="7af80-128">You can create a Linux VM using the popular UbuntuLTS image, with two attached storage disks of 10 GB and 20 GB, with the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

<span data-ttu-id="7af80-129">Quand vous exécutez la commande précédente, Azure CLI 2.0 recherche une paire de clés SSH stockée dans votre répertoire ~/.ssh.</span><span class="sxs-lookup"><span data-stu-id="7af80-129">When you run the preceding command, the Azure CLI 2.0 looks for an SSH key pair stored under your ~/.ssh directory.</span></span>  <span data-ttu-id="7af80-130">Si aucune paire de clés SSH n’est encore stockée à cet emplacement, vous pouvez demander à Azure CLI d’en créer automatiquement une pour vous en passant le paramètre --generate-ssh-keys :</span><span class="sxs-lookup"><span data-stu-id="7af80-130">If you don't already have an SSH key pair stored there, you can ask the Azure CLI to automatically create one for you by passing the --generate-ssh-keys parameter:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

<span data-ttu-id="7af80-131">La commande `az vm create` retourne un résultat une fois la machine virtuelle entièrement créée, accessible et utilisable.</span><span class="sxs-lookup"><span data-stu-id="7af80-131">The `az vm create` command returns output once the VM has been fully created and is ready to be accessed and used.</span></span> <span data-ttu-id="7af80-132">La sortie contient plusieurs propriétés de la nouvelle machine virtuelle, notamment son adresse IP publique :</span><span class="sxs-lookup"><span data-stu-id="7af80-132">The output includes several properties of the newly created VM including its public IP address:</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="7af80-133">Vous pouvez maintenant vous connecter à votre nouvelle machine virtuelle Linux à l’aide de **SSH** avec l’adresse IP publique de la machine virtuelle que vous avez créée :</span><span class="sxs-lookup"><span data-stu-id="7af80-133">Now that the VM has been created, you can log on to your new Linux VM using **SSH** with the public IP address of the VM you created:</span></span>

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a><span data-ttu-id="7af80-134">Créer une machine virtuelle Windows Server</span><span class="sxs-lookup"><span data-stu-id="7af80-134">Create a Windows Server Virtual Machine</span></span>

<span data-ttu-id="7af80-135">Nous allons maintenant créer une machine virtuelle Windows Server 2016 Datacenter à l’aide de la commande `az vm create`, puis l’ajouter au groupe de ressources « MyResourceGroup » que nous avons utilisé pour notre machine virtuelle Linux.</span><span class="sxs-lookup"><span data-stu-id="7af80-135">Let's now create a Windows Server 2016 Datacenter-based VM using the `az vm create` command and add it to the same "MyResourceGroup" resource group that we used for our Linux VM.</span></span>  <span data-ttu-id="7af80-136">Comme pour l’exemple de machine virtuelle Linux, nous allons attacher deux disques de stockage à l’aide du paramètre `--data-disk-sizes-gb`.</span><span class="sxs-lookup"><span data-stu-id="7af80-136">Like the Linux VM example, we'll also attach two storage disks using the `--data-disk-sizes-gb` parameter.</span></span>

<span data-ttu-id="7af80-137">Azure vous demande d’éviter d’utiliser des noms d’utilisateur/mots de passe faciles à deviner.</span><span class="sxs-lookup"><span data-stu-id="7af80-137">Azure requires that you avoid using easily guessed usernames/passwords.</span></span> <span data-ttu-id="7af80-138">Il existe des règles spécifiques sur les caractères pouvant être utilisés et sur la longueur minimale du nom d’utilisateur et du mot de passe.</span><span class="sxs-lookup"><span data-stu-id="7af80-138">There are specific rules for what characters can be used as well as the minimum length of both username and password.</span></span>

> [!NOTE]
> <span data-ttu-id="7af80-139">Vous serez invité à entrer votre nom d’utilisateur et votre mot de passe lors de l’exécution de cette commande.</span><span class="sxs-lookup"><span data-stu-id="7af80-139">You will be prompted to enter your username and password when running this command.</span></span>

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

<span data-ttu-id="7af80-140">La commande `az vm create` retourne un résultat une fois la machine virtuelle entièrement créée, accessible et utilisable.</span><span class="sxs-lookup"><span data-stu-id="7af80-140">The `az vm create` command output results once the VM has been fully created and is ready to be accessed and used.</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="7af80-141">Connectez-vous maintenant à la machine virtuelle Windows Server que vous venez de créer à l’aide du Bureau à distance et de l’adresse IP publique de la machine virtuelle (qui est retournée dans la sortie de `az vm create`).</span><span class="sxs-lookup"><span data-stu-id="7af80-141">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM (which is returned in the output from `az vm create`).</span></span>
<span data-ttu-id="7af80-142">Si vous êtes sur un système Windows, vous pouvez pour cela exécuter la commande `mstsc` à partir de la ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="7af80-142">If you are on a Windows-based system, you can do this from the command line using the `mstsc` command:</span></span>

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="7af80-143">Fournissez la même combinaison de nom d’utilisateur/mot de passe que celle que vous avez utilisée lors de la création de la machine virtuelle pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="7af80-143">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="7af80-144">Création d’autres ressources dans Azure</span><span class="sxs-lookup"><span data-stu-id="7af80-144">Creating other resources in Azure</span></span>

<span data-ttu-id="7af80-145">Nous avons vu comment créer un groupe de ressources, une machine virtuelle Linux et une machine virtuelle Windows Server.</span><span class="sxs-lookup"><span data-stu-id="7af80-145">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="7af80-146">Vous pouvez créer de nombreux autres types de ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-146">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="7af80-147">Toutes les nouvelles ressources sont créées à l’aide d’un modèle de nommage `az <resource type name> create` cohérent.</span><span class="sxs-lookup"><span data-stu-id="7af80-147">All new resources are created using a consistent `az <resource type name> create` naming pattern.</span></span>  <span data-ttu-id="7af80-148">Par exemple, pour créer un équilibreur de charge réseau Azure que nous pourrions ensuite associer avec nos nouvelles machines virtuelles, nous pouvons utiliser la commande create suivante :</span><span class="sxs-lookup"><span data-stu-id="7af80-148">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

<span data-ttu-id="7af80-149">Nous pourrions aussi créer un réseau privé virtuel (communément appelé « VNet » dans Azure) pour notre infrastructure à l’aide de la commande create suivante :</span><span class="sxs-lookup"><span data-stu-id="7af80-149">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following create command:</span></span>

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

<span data-ttu-id="7af80-150">Ce qui rend Azure et Azure CLI si puissants, c’est que nous pouvons les utiliser non seulement pour obtenir une infrastructure cloud, mais également pour créer des services de plateforme gérés.</span><span class="sxs-lookup"><span data-stu-id="7af80-150">What makes Azure and the Azure CLI powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span>  <span data-ttu-id="7af80-151">Les services de plateforme gérés peuvent aussi être combinés avec l’infrastructure pour générer des solutions encore plus puissantes.</span><span class="sxs-lookup"><span data-stu-id="7af80-151">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="7af80-152">Par exemple, vous pouvez utiliser Azure CLI pour créer un service Azure App Service.</span><span class="sxs-lookup"><span data-stu-id="7af80-152">For example, you can use the Azure CLI to create an Azure AppService.</span></span>  <span data-ttu-id="7af80-153">Azure App Service est un service de plateforme géré qui offre un excellent moyen d’héberger des applications web sans avoir à se soucier de l’infrastructure.</span><span class="sxs-lookup"><span data-stu-id="7af80-153">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span>  <span data-ttu-id="7af80-154">Après avoir créé le service Azure App Service, vous pouvez créer deux nouvelles applications web Azure dans l’App Service à l’aide des commandes create suivantes :</span><span class="sxs-lookup"><span data-stu-id="7af80-154">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following create commands:</span></span>

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan
```

<span data-ttu-id="7af80-155">Une fois que vous avez compris les principes fondamentaux du modèle `az <resource type name> create`, il devient facile de créer tout ce que vous voulez.</span><span class="sxs-lookup"><span data-stu-id="7af80-155">Once you understand the basics of the `az <resource type name> create` pattern, it becomes easy to create anything.</span></span> <span data-ttu-id="7af80-156">Voici quelques types de ressources Azure populaires et les commandes create Azure CLI correspondantes pour les créer :</span><span class="sxs-lookup"><span data-stu-id="7af80-156">Following are some popular Azure resource types and the corresponding Azure CLI create commands to create them:</span></span>

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

<span data-ttu-id="7af80-157">Consultez la [documentation de référence](/cli/azure) pour en savoir plus sur les paramètres propres aux ressources supplémentaires que vous pouvez passer à chacune des commandes précédentes et sur les types de ressources que vous pouvez créer.</span><span class="sxs-lookup"><span data-stu-id="7af80-157">Visit the [Reference documentation](/cli/azure) to learn more about the additional resource-specific parameters that you can pass to each of the preceding commands and the resource types you can create.</span></span>

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a><span data-ttu-id="7af80-158">Astuce : Optimisation des opérations de création à l’aide de --no-wait</span><span class="sxs-lookup"><span data-stu-id="7af80-158">Useful tip: Optimizing create operations using --no-wait</span></span>

<span data-ttu-id="7af80-159">Par défaut, quand vous créez des ressources à l’aide d’Azure CLI 2.0, la commande `az <resource type name> create` attend que la ressource ait été créée et soit prête à l’emploi.</span><span class="sxs-lookup"><span data-stu-id="7af80-159">By default when you create resources using the Azure CLI 2.0, the `az <resource type name> create` command waits until the resource has been created and is ready for you to use.</span></span>  <span data-ttu-id="7af80-160">Par exemple, si vous créez une machine virtuelle, la commande `az vm create`, par défaut, ne retourne qu’une fois la machine virtuelle créée et prête à ce que vous y accédiez par SSH ou RDP.</span><span class="sxs-lookup"><span data-stu-id="7af80-160">For example, if you create a VM, the `az vm create` command will, by default, not return until the VM is created and is ready for you to SSH or RDP into it.</span></span>

<span data-ttu-id="7af80-161">Nous adoptons cette approche car elle facilite l’écriture des scripts d’automatisation qui contiennent plusieurs étapes avec des dépendances (et qui ont besoin qu’une tâche précédente soit terminée avant de continuer).</span><span class="sxs-lookup"><span data-stu-id="7af80-161">We use this approach because it makes it easier to write automation scripts that contain multiple steps with dependencies (and need a prior task to have completed successfully before continuing).</span></span>

<span data-ttu-id="7af80-162">Si vous n’avez pas besoin d’attendre lors de la création d’une ressource, vous pouvez utiliser l’option `no-wait` pour démarrer une action de création en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="7af80-162">If you do not need to wait on creation of a resource before continuing, you can use the `no-wait` option to start a create action in the background.</span></span> <span data-ttu-id="7af80-163">Vous pouvez continuer à utiliser l’interface de ligne de commande pour d’autres commandes.</span><span class="sxs-lookup"><span data-stu-id="7af80-163">You can continue using the CLI for other commands.</span></span>

<span data-ttu-id="7af80-164">Par exemple, la commande `az vm create` ci-dessous démarre un déploiement de machine virtuelle, puis retourne beaucoup plus rapidement (et avant que la machine virtuelle ait démarré complètement) :</span><span class="sxs-lookup"><span data-stu-id="7af80-164">For example, the following usage of the `az vm create` starts a VM deployment and then return much more quickly (and before the VM has fully booted):</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

<span data-ttu-id="7af80-165">`--no-wait` peut vous aider à optimiser sensiblement les performances de vos scripts d’automatisation.</span><span class="sxs-lookup"><span data-stu-id="7af80-165">Using the `--no-wait` approach can help you optimize the performance of your automation scripts considerably.</span></span>

## <a name="listing-resources-and-formatting-output"></a><span data-ttu-id="7af80-166">Liste des ressources et mise en forme de la sortie</span><span class="sxs-lookup"><span data-stu-id="7af80-166">Listing resources and formatting output</span></span>

<span data-ttu-id="7af80-167">Vous pouvez utiliser la commande `list` dans Azure CLI pour rechercher et lister les ressources en cours d’exécution dans Azure.</span><span class="sxs-lookup"><span data-stu-id="7af80-167">You can use the `list` command within the Azure CLI to find and list the resources running in Azure.</span></span>

<span data-ttu-id="7af80-168">Comme avec la commande create, vous pouvez lister les ressources à l’aide d’Azure CLI 2.0 avec un modèle de nommage `az <resource type name> list` commun et cohérent entre tous les types de ressources.</span><span class="sxs-lookup"><span data-stu-id="7af80-168">Like with the create command, you can list resources using the Azure CLI 2.0 using a common `az <resource type name> list` naming pattern that is consistent across all resource types.</span></span>  <span data-ttu-id="7af80-169">Différents formats de sortie et options de requête sont disponibles pour filtrer et trier la liste des ressources à votre goût.</span><span class="sxs-lookup"><span data-stu-id="7af80-169">There are various output formats and query options available to filter and sort the list of resources in the way you prefer to see them.</span></span>

<span data-ttu-id="7af80-170">Par exemple, `az vm list` affiche la liste de toutes vos machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="7af80-170">For example, `az vm list` shows the list of all VMs you have.</span></span>

```azurecli-interactive
az vm list
```
<span data-ttu-id="7af80-171">Les valeurs retournées sont par défaut au format JSON (affichant uniquement une sortie partielle, par souci de clarté).</span><span class="sxs-lookup"><span data-stu-id="7af80-171">The values returned are by default in JSON (only showing partial output for sake of brevity).</span></span>

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...
]
```

<span data-ttu-id="7af80-172">Vous pouvez modifier le format de sortie à l’aide de l’option `--output`.</span><span class="sxs-lookup"><span data-stu-id="7af80-172">You can optionally modify the output format using the `--output` option.</span></span>  <span data-ttu-id="7af80-173">Exécutez la commande `az vm list` pour afficher les machines virtuelles Linux et Windows Server créées précédemment, ainsi que les propriétés les plus courantes d’une machine virtuelle, à l’aide de l’option de format *table* facile à lire :</span><span class="sxs-lookup"><span data-stu-id="7af80-173">Run the `az vm list` command to see both the Linux and Windows Server VMs created earlier, along with the most common properties of a VM, using the easy to read *table* format option:</span></span>

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="7af80-174">Vous pouvez utiliser l’option de sortie *tsv* pour obtenir un format textuel de valeurs séparées par des tabulations, sans en-tête.</span><span class="sxs-lookup"><span data-stu-id="7af80-174">The *tsv* output option can be used to get a text-based, tab-separated format without any headers.</span></span>  <span data-ttu-id="7af80-175">Ce format est utile quand vous souhaitez diriger la sortie vers un autre outil texte comme grep.</span><span class="sxs-lookup"><span data-stu-id="7af80-175">This format is useful when you want to pipe the output into another text-based tool like grep.</span></span>

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
<span data-ttu-id="7af80-176">Consultez l’article sur les [formats de sortie](format-output-azure-cli.md) pour en savoir plus sur les autres méthodes permettant de lister les ressources et de mettre en forme la sortie.</span><span class="sxs-lookup"><span data-stu-id="7af80-176">Visit the [output formats](format-output-azure-cli.md) article to learn more about the additional ways to list resources and format the output.</span></span>

## <a name="querying-resources-and-shaping-outputs"></a><span data-ttu-id="7af80-177">Interrogation de ressources et mise en forme des sorties</span><span class="sxs-lookup"><span data-stu-id="7af80-177">Querying resources and shaping outputs</span></span>

<span data-ttu-id="7af80-178">Souvent, vous souhaitez pouvoir interroger uniquement les ressources qui remplissent une condition spécifique.</span><span class="sxs-lookup"><span data-stu-id="7af80-178">Often you want to be able to query for only those resources that meet a specific condition.</span></span>

<span data-ttu-id="7af80-179">La commande `list` offre une prise en charge intégrée qui simplifie le filtrage des ressources par nom de groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="7af80-179">The `list` command has built-in support that makes it easy to filter resources by Resource Group name.</span></span>  <span data-ttu-id="7af80-180">Par exemple, vous pouvez passer un paramètre `--ResourceGroup` ou `-g` à une commande `list` pour récupérer uniquement les ressources appartenant à un groupe de ressources spécifique :</span><span class="sxs-lookup"><span data-stu-id="7af80-180">For example, you can pass either a `--ResourceGroup` or `-g` parameter to a `list` command to only retrieve those resources within a specific resource group:</span></span>


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="7af80-181">Pour des requêtes encore plus poussées, vous pouvez utiliser le paramètre `--query` pour exécuter une requête JMESPath sur les résultats de *n’importe quelle* commande `az`.</span><span class="sxs-lookup"><span data-stu-id="7af80-181">For even more powerful querying support, you can use the `--query` parameter to execute a JMESPath query on the results of *any* `az` command.</span></span>  <span data-ttu-id="7af80-182">Vous pouvez utiliser des requêtes JMESPath pour filtrer et mettre en forme la sortie de n’importe quel résultat retourné.</span><span class="sxs-lookup"><span data-stu-id="7af80-182">JMESPath queries can be used both to filter as well as shape the output of any returned result.</span></span>

<span data-ttu-id="7af80-183">Par exemple, exécutez la commande suivante pour rechercher les ressources de machine virtuelle dans tous les groupes de ressources qui contiennent les lettres « My » :</span><span class="sxs-lookup"><span data-stu-id="7af80-183">For example, execute the following command to query for any VM resource within any resource group that contains the letters "My":</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')]"
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="7af80-184">Ensuite, nous pouvons choisir d’affiner davantage la sortie en exploitant la fonctionnalité de mise en forme des requêtes JMESPath pour générer des valeurs différentes.</span><span class="sxs-lookup"><span data-stu-id="7af80-184">We could then choose to further refine the output by using the shaping capability of JMESPath queries to output different values as well.</span></span>  <span data-ttu-id="7af80-185">Par exemple, la commande suivante récupère le type de disque de système d’exploitation utilisé par la machine virtuelle afin de déterminer s’il s’agit d’un système d’exploitation Linux ou Windows :</span><span class="sxs-lookup"><span data-stu-id="7af80-185">For example, the following command retrieves the type of OS disk the VM is using to determine whether the OS is Linux or Windows based:</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')].{ VMName:name, OSType:storageProfile.osDisk.osType }"
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

<span data-ttu-id="7af80-186">La prise en charge de JMESPath dans Azure CLI est puissante.</span><span class="sxs-lookup"><span data-stu-id="7af80-186">The JMESPath support in Azure CLI is powerful.</span></span>  <span data-ttu-id="7af80-187">Pour en savoir plus sur son utilisation, consultez notre article sur les [requêtes](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7af80-187">Learn more about how to use it in our [query](query-azure-cli.md) article.</span></span>

## <a name="deleting-resources"></a><span data-ttu-id="7af80-188">Suppression de ressources</span><span class="sxs-lookup"><span data-stu-id="7af80-188">Deleting resources</span></span>

<span data-ttu-id="7af80-189">Vous pouvez utiliser la commande `delete` dans Azure CLI pour supprimer les ressources dont vous n’avez plus besoin.</span><span class="sxs-lookup"><span data-stu-id="7af80-189">You can use the `delete` command within Azure CLI to delete the resources you no longer need.</span></span> <span data-ttu-id="7af80-190">Vous pouvez utiliser la commande `delete` avec n’importe quelle ressource, comme avec la commande `create`.</span><span class="sxs-lookup"><span data-stu-id="7af80-190">You can use the `delete` command with any resource just like you can with the `create` command.</span></span>

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

<span data-ttu-id="7af80-191">Par défaut, l’interface de ligne de commande vous invite à confirmer la suppression.</span><span class="sxs-lookup"><span data-stu-id="7af80-191">By default the CLI prompts to confirm deletion.</span></span>  <span data-ttu-id="7af80-192">Vous pouvez supprimer cette invite pour les scripts automatisés.</span><span class="sxs-lookup"><span data-stu-id="7af80-192">You can suppress this prompt for automated scripts.</span></span>

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

<span data-ttu-id="7af80-193">Vous pouvez aussi utiliser la commande `delete` pour supprimer de nombreuses ressources à la fois.</span><span class="sxs-lookup"><span data-stu-id="7af80-193">You can also use the `delete` command to delete many resources at a time.</span></span> <span data-ttu-id="7af80-194">Par exemple, la commande suivante supprime toutes les ressources du groupe de ressources « MyResourceGroup » que nous avons utilisées pour tous les exemples de ce didacticiel.</span><span class="sxs-lookup"><span data-stu-id="7af80-194">For example, the following command deletes all the resources in the "MyResourceGroup" resource group that we've used for all the samples in this Get Started tutorial.</span></span>

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a><span data-ttu-id="7af80-195">Obtenir les exemples</span><span class="sxs-lookup"><span data-stu-id="7af80-195">Get samples</span></span>

<span data-ttu-id="7af80-196">Pour plus d’informations sur les différentes façons d’utiliser Azure CLI, découvrez nos scripts les plus courants pour les [machines virtuelles Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), les [machines virtuelles Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), les [applications web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) et les [bases de données SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="7af80-196">To learn more about ways to use the Azure CLI, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), and [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span></span>

## <a name="read-the-api-reference-docs"></a><span data-ttu-id="7af80-197">Lire la documentation de référence sur les API</span><span class="sxs-lookup"><span data-stu-id="7af80-197">Read the API reference docs</span></span>

[<span data-ttu-id="7af80-198">Informations de référence sur les API</span><span class="sxs-lookup"><span data-stu-id="7af80-198">API reference</span></span>](/cli/azure)

## <a name="get-help"></a><span data-ttu-id="7af80-199">Obtenir de l’aide</span><span class="sxs-lookup"><span data-stu-id="7af80-199">Get help</span></span>

<span data-ttu-id="7af80-200">Azure CLI contient une documentation d’aide intégrée, qui correspond à notre documentation web que vous pouvez exécuter à partir de la ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="7af80-200">The Azure CLI has built-in help documentation, which matches our web documentation that you can run from the command line:</span></span>

```azurecli-interactive
az [command-group [command]] -h
```

<span data-ttu-id="7af80-201">Par exemple, pour afficher les sous-groupes et les commandes disponibles pour les machines virtuelles, exécutez :</span><span class="sxs-lookup"><span data-stu-id="7af80-201">For example, to see what commands and subgroups are available for VMs, use:</span></span>

```azurecli-interactive
az vm -h
```

<span data-ttu-id="7af80-202">Pour obtenir de l’aide avec la commande de création de machine virtuelle, exécutez :</span><span class="sxs-lookup"><span data-stu-id="7af80-202">To get help with the command to create a VM, use:</span></span>

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a><span data-ttu-id="7af80-203">Transition à partir d’Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="7af80-203">Switch from Azure CLI 1.0</span></span>

<span data-ttu-id="7af80-204">Si vous savez déjà comment utiliser Azure CLI 1.0 (azure.js), vous remarquerez certains emplacements où les commandes ne sont pas identiques.</span><span class="sxs-lookup"><span data-stu-id="7af80-204">If you already know how to use Azure CLI 1.0 (azure.js), you'll notice places where the commands aren't quite the same.</span></span>
<span data-ttu-id="7af80-205">Parfois, les commandes pour effectuer une tâche sont très différentes.</span><span class="sxs-lookup"><span data-stu-id="7af80-205">Sometimes the commands to perform a task are significantly different.</span></span>
<span data-ttu-id="7af80-206">Pour vous aider à passer d’Azure CLI 1.0 à Azure CLI 2.0, nous avons commencé cette [mise en correspondance des commandes](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span><span class="sxs-lookup"><span data-stu-id="7af80-206">To help you make the switch from Azure CLI 1.0 to Azure CLI 2.0, we've started this [command mapping](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span></span>

## <a name="send-us-your-feedback"></a><span data-ttu-id="7af80-207">Envoyez-nous vos commentaires</span><span class="sxs-lookup"><span data-stu-id="7af80-207">Send us your feedback</span></span>

```azurecli-interactive
az feedback
```
