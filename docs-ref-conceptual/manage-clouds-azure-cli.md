---
title: "La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0"
description: "Créer, se connecter et gérer plusieurs clouds avec l’interface de ligne de commande Azure 2.0."
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: ee6b1b6b1e611229ba6e6e0c4b2ca2de6f7ceaee
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="03a66-103">La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="03a66-103">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="03a66-104">Si vous travaillez sur différentes régions ou utilisez [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), vous devrez peut-être utiliser plusieurs clouds.</span><span class="sxs-lookup"><span data-stu-id="03a66-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="03a66-105">Microsoft fournit des clouds conformes aux lois régionales, qui sont à votre disposition.</span><span class="sxs-lookup"><span data-stu-id="03a66-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="03a66-106">Cet article explique comment obtenir des informations sur les clouds disponibles sur votre compte, modifier le cloud actuel, et inscrire ou annuler désinscrire nouveaux clouds à utiliser avec Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="03a66-106">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="03a66-107">Énumération des clouds</span><span class="sxs-lookup"><span data-stu-id="03a66-107">Listing clouds</span></span>

<span data-ttu-id="03a66-108">Vous pouvez lister les clouds disponibles avec la commande [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="03a66-108">You can list available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="03a66-109">Elle indique quel cloud est actuellement actif, son profil actuel, et fournit des informations sur les noms d’hôte et les suffixes régionaux.</span><span class="sxs-lookup"><span data-stu-id="03a66-109">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="03a66-110">Pour obtenir le cloud actif et une liste de tous les clouds disponibles :</span><span class="sxs-lookup"><span data-stu-id="03a66-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

<span data-ttu-id="03a66-111">Le cloud actuellement actif a `True` dans la colonne `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="03a66-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="03a66-112">Un seul cloud peut être actif à tout moment.</span><span class="sxs-lookup"><span data-stu-id="03a66-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="03a66-113">Pour obtenir des informations plus détaillées sur un cloud, y compris sur les points de terminaison qu’il utilise pour les services Azure, utilisez la commande `cloud show` :</span><span class="sxs-lookup"><span data-stu-id="03a66-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a><span data-ttu-id="03a66-114">Changement du cloud actif</span><span class="sxs-lookup"><span data-stu-id="03a66-114">Switching the active cloud</span></span>

<span data-ttu-id="03a66-115">Pour changer le cloud actuellement actif, exécutez la commande [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="03a66-115">To switch the currently active cloud, run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="03a66-116">Cette commande accepte un argument obligatoire, qui est le nom du cloud.</span><span class="sxs-lookup"><span data-stu-id="03a66-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="03a66-117">Si l’authentification pour le cloud activé a expiré, vous devez vous authentifier de nouveau avant d’effectuer d’autres tâches CLI.</span><span class="sxs-lookup"><span data-stu-id="03a66-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="03a66-118">S’il s’agit de la première fois que vous changez vers le nouveau cloud, vous devez également configurer l’abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="03a66-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="03a66-119">Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec l’interface de ligne de commande Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="03a66-119">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="03a66-120">Pour plus d’informations sur la gestion des abonnements, consultez [Gestion des abonnements Azure avec Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="03a66-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="03a66-121">Inscrire un cloud</span><span class="sxs-lookup"><span data-stu-id="03a66-121">Register a cloud</span></span>

<span data-ttu-id="03a66-122">Inscrivez un nouveau cloud si vous disposez de vos propres points de terminaison pour Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="03a66-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="03a66-123">La création d’un cloud s’effectue avec la commande [cloud register](/cli/azure/cloud#register) .</span><span class="sxs-lookup"><span data-stu-id="03a66-123">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="03a66-124">Cette commande nécessite un nom et un ensemble de fonctionnalités avec les points de terminaison associés.</span><span class="sxs-lookup"><span data-stu-id="03a66-124">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="03a66-125">Pour savoir comment inscrire un cloud pour une utilisation avec Azure Stack, consultez [Installer et configurer CLI pour une utilisation avec Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="03a66-125">To learn how to register a cloud for use with Azure Stack, see [Install and configure CLI for use with Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span></span>

<span data-ttu-id="03a66-126">Vous n’avez pas besoin d’inscrire votre propre cloud pour les régions de la Chine, du Gouvernement des États-Unis ou de l’Allemagne.</span><span class="sxs-lookup"><span data-stu-id="03a66-126">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="03a66-127">Celles-ci sont gérées par Microsoft et disponibles par défaut.</span><span class="sxs-lookup"><span data-stu-id="03a66-127">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="03a66-128">Pour plus d’informations sur tous les paramètres de point de terminaison disponibles, consultez la [documentation pour `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span><span class="sxs-lookup"><span data-stu-id="03a66-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span></span>

<span data-ttu-id="03a66-129">L’inscription d’un cloud n’active pas automatiquement ce dernier.</span><span class="sxs-lookup"><span data-stu-id="03a66-129">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="03a66-130">Utilisez la commande `az cloud set` pour sélectionner le cloud qui vient d’être créé comme décrit ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="03a66-130">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="03a66-131">Mettre à jour un cloud existant</span><span class="sxs-lookup"><span data-stu-id="03a66-131">Update an existing cloud</span></span>

<span data-ttu-id="03a66-132">Si vous disposez des autorisations, vous pouvez également mettre à jour un cloud existant.</span><span class="sxs-lookup"><span data-stu-id="03a66-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="03a66-133">Faites-le lorsque vous avez besoin de basculer vers un autre profil Azure, ou d’ajouter ou de modifier un point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="03a66-133">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="03a66-134">Faites-le avec la commande `az cloud update`, qui accepte les mêmes arguments que `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="03a66-134">You do this with the `az cloud update` command, which takes the same arguments as `az cloud register`.</span></span> <span data-ttu-id="03a66-135">Pour plus d’informations, consultez la [documentation pour `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span><span class="sxs-lookup"><span data-stu-id="03a66-135">For more information, see the [documentation for `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="03a66-136">Désinscrire un cloud</span><span class="sxs-lookup"><span data-stu-id="03a66-136">Unregister a cloud</span></span>

<span data-ttu-id="03a66-137">Si vous n’avez plus besoin d’un cloud inscrit, vous pouvez le désinscrire avec la commande [cloud unregister](/cli/azure/cloud#unregister) :</span><span class="sxs-lookup"><span data-stu-id="03a66-137">If you no longer require a registered cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```
