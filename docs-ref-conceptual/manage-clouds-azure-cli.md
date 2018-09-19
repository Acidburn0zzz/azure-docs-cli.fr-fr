---
title: Sélectionnez les clouds avec Azure CLI 2.0
description: Créer, se connecter et gérer plusieurs clouds avec l’interface de ligne de commande Azure 2.0.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 26b9f414ddaba3cc3f834b4749dee9807d84aa79
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388403"
---
# <a name="select-clouds-with-azure-cli-20"></a><span data-ttu-id="4e44b-103">Sélectionnez les clouds avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="4e44b-103">Select clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="4e44b-104">Si vous travaillez sur différentes régions ou utilisez [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), vous devrez peut-être utiliser plusieurs clouds.</span><span class="sxs-lookup"><span data-stu-id="4e44b-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="4e44b-105">Microsoft fournit des clouds conformes aux lois régionales, qui sont à votre disposition.</span><span class="sxs-lookup"><span data-stu-id="4e44b-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="4e44b-106">Cet article vous explique comment obtenir des informations sur les clouds, modifier le cloud actuel, et inscrire ou désinscrire de nouveaux clouds.</span><span class="sxs-lookup"><span data-stu-id="4e44b-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="4e44b-107">Répertorier les clouds disponibles</span><span class="sxs-lookup"><span data-stu-id="4e44b-107">List available clouds</span></span>

<span data-ttu-id="4e44b-108">Vous pouvez lister les clouds disponibles avec la commande [az cloud list](/cli/azure/cloud#az-cloud-list).</span><span class="sxs-lookup"><span data-stu-id="4e44b-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="4e44b-109">Cette commande indique quel cloud est actuellement actif, quel est son profil actuel, et elle fournit des informations concernant les noms d’hôte et les suffixes régionaux.</span><span class="sxs-lookup"><span data-stu-id="4e44b-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="4e44b-110">Pour obtenir le cloud actif et une liste de tous les clouds disponibles :</span><span class="sxs-lookup"><span data-stu-id="4e44b-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
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

<span data-ttu-id="4e44b-111">Le cloud actuellement actif a `True` dans la colonne `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="4e44b-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="4e44b-112">Un seul cloud peut être actif à tout moment.</span><span class="sxs-lookup"><span data-stu-id="4e44b-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="4e44b-113">Pour obtenir des informations plus détaillées sur un cloud, y compris sur les points de terminaison qu’il utilise pour les services Azure, utilisez la commande `cloud show` :</span><span class="sxs-lookup"><span data-stu-id="4e44b-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
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

## <a name="switch-the-active-cloud"></a><span data-ttu-id="4e44b-114">Changer de cloud actif</span><span class="sxs-lookup"><span data-stu-id="4e44b-114">Switch the active cloud</span></span>

<span data-ttu-id="4e44b-115">Pour changer le cloud actuellement actif, exécutez la commande [az cloud set](/cli/azure/cloud#az-cloud-set).</span><span class="sxs-lookup"><span data-stu-id="4e44b-115">To switch the currently active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="4e44b-116">Cette commande accepte un argument obligatoire, qui est le nom du cloud.</span><span class="sxs-lookup"><span data-stu-id="4e44b-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="4e44b-117">Si l’authentification pour le cloud activé a expiré, vous devez vous authentifier de nouveau avant d’effectuer d’autres tâches CLI.</span><span class="sxs-lookup"><span data-stu-id="4e44b-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="4e44b-118">S’il s’agit de la première fois que vous changez vers le nouveau cloud, vous devez également configurer l’abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="4e44b-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="4e44b-119">Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec l’interface de ligne de commande Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="4e44b-119">For instructions on authenticating, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="4e44b-120">Pour plus d’informations sur la gestion des abonnements, consultez [Gestion des abonnements Azure avec Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="4e44b-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="4e44b-121">Inscrire un nouveau cloud</span><span class="sxs-lookup"><span data-stu-id="4e44b-121">Register a new cloud</span></span>

<span data-ttu-id="4e44b-122">Inscrivez un nouveau cloud si vous disposez de vos propres points de terminaison pour Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4e44b-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="4e44b-123">La création d’un cloud s’effectue avec la commande [az cloud register](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="4e44b-123">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="4e44b-124">Cette commande nécessite un nom et un ensemble de points de terminaison de service.</span><span class="sxs-lookup"><span data-stu-id="4e44b-124">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="4e44b-125">Pour savoir comment inscrire un cloud pour une utilisation avec Azure Stack, consultez [Utiliser des profils de version des API avec Azure CLI 2.0 dans Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="4e44b-125">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI 2.0 in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="4e44b-126">Vous n’avez pas besoin d’inscrire votre propre cloud pour les régions de la Chine, du gouvernement des États-Unis ou de l’Allemagne.</span><span class="sxs-lookup"><span data-stu-id="4e44b-126">You do don't to register your own cloud for the China, US Government, or German regions.</span></span> <span data-ttu-id="4e44b-127">Ces clouds sont gérés par Microsoft et disponibles par défaut.</span><span class="sxs-lookup"><span data-stu-id="4e44b-127">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="4e44b-128">Pour plus d’informations sur tous les paramètres de point de terminaison disponibles, consultez la [documentation pour `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="4e44b-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="4e44b-129">L’inscription d’un cloud n’active pas automatiquement ce dernier.</span><span class="sxs-lookup"><span data-stu-id="4e44b-129">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="4e44b-130">Utilisez la commande `az cloud set` pour sélectionner le cloud récemment créé.</span><span class="sxs-lookup"><span data-stu-id="4e44b-130">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="4e44b-131">Mettre à jour un cloud existant</span><span class="sxs-lookup"><span data-stu-id="4e44b-131">Update an existing cloud</span></span>

<span data-ttu-id="4e44b-132">Si vous disposez des autorisations, vous pouvez également mettre à jour un cloud existant.</span><span class="sxs-lookup"><span data-stu-id="4e44b-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="4e44b-133">La mise à jour d’un cloud bascule vers un profil de services Azure différent, ou modifie les points de terminaison de connexion.</span><span class="sxs-lookup"><span data-stu-id="4e44b-133">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="4e44b-134">Mettez à jour un cloud avec la commande [az cloud update](/cli/azure/cloud#az-cloud-update), qui accepte les mêmes arguments que `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="4e44b-134">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="4e44b-135">Désinscrire un cloud</span><span class="sxs-lookup"><span data-stu-id="4e44b-135">Unregister a cloud</span></span>

<span data-ttu-id="4e44b-136">Si vous n’avez plus besoin du cloud créé, il peut être désinscrit avec la commande [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) :</span><span class="sxs-lookup"><span data-stu-id="4e44b-136">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```
