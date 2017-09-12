---
title: "La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0"
description: "Créer, se connecter et gérer plusieurs clouds avec l’interface de ligne de commande Azure 2.0."
keywords: "Interface de ligne de commande Azure 2.0, Azure, clouds, centres de données, gouvernement, région, Chine, Allemagne"
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="dcee8-104">La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="dcee8-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="dcee8-105">Si vous avez plusieurs abonnements associés à Azure, il se peut que vous ayez plusieurs cloud disponibles.</span><span class="sxs-lookup"><span data-stu-id="dcee8-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="dcee8-106">Chaque cloud a ses propres points de terminaison associés et ses propres capacités. Ils sont souvent associés à une région particulière qui a des normes de protection de données ou des configurations différentes.</span><span class="sxs-lookup"><span data-stu-id="dcee8-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="dcee8-107">Pour travailler efficacement avec plusieurs clouds, vous devez être en mesure de basculer entre ceux qui sont actuellement actifs et éventuellement créer de nouveaux clouds.</span><span class="sxs-lookup"><span data-stu-id="dcee8-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="dcee8-108">Énumération des clouds</span><span class="sxs-lookup"><span data-stu-id="dcee8-108">Listing clouds</span></span>

<span data-ttu-id="dcee8-109">Vous pouvez énumérer vos clouds disponibles avec la commande [liste des clouds](/cli/azure/cloud#list) .</span><span class="sxs-lookup"><span data-stu-id="dcee8-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="dcee8-110">Cela indique le cloud actuellement actif, son profil actuel et vous fournit des informations sur les noms d’hôte et les suffixes régionaux.</span><span class="sxs-lookup"><span data-stu-id="dcee8-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="dcee8-111">Pour obtenir une liste des clouds disponibles et de celui qui est actuellement actif :</span><span class="sxs-lookup"><span data-stu-id="dcee8-111">To get a list of the available clouds and the currently active one:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="dcee8-112">Changement du cloud actif</span><span class="sxs-lookup"><span data-stu-id="dcee8-112">Switching the active cloud</span></span>

<span data-ttu-id="dcee8-113">Pour basculer le cloud actuellement actif, vous devez exécuter la commande [ensemble de clouds](/cli/azure/cloud#set) .</span><span class="sxs-lookup"><span data-stu-id="dcee8-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="dcee8-114">Cette commande accepte un argument obligatoire, qui est le nom du cloud.</span><span class="sxs-lookup"><span data-stu-id="dcee8-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="dcee8-115">Si vous n’avez jamais effectué d’authentification pour le cloud actif, vous devez le faire avant d’effectuer d’autres opérations de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="dcee8-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="dcee8-116">Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec l’interface de ligne de commande Azure 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="dcee8-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="dcee8-117">Inscrire ou désinscrire un cloud</span><span class="sxs-lookup"><span data-stu-id="dcee8-117">Register or unregister a cloud</span></span>

<span data-ttu-id="dcee8-118">Inscrire un nouveau cloud si vous avez vos propres points de terminaison ou si vous avez besoin d’un profil différent.</span><span class="sxs-lookup"><span data-stu-id="dcee8-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="dcee8-119">La création d’un cloud s’effectue avec la commande [cloud register](/cli/azure/cloud#register) .</span><span class="sxs-lookup"><span data-stu-id="dcee8-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="dcee8-120">Cette commande nécessite un nom et éventuellement un ensemble de configurations et de désignations de point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="dcee8-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="dcee8-121">Pour créer un cloud avec un point de terminaison spécialisé pour le gestionnaire de ressources, avec un profil spécifique :</span><span class="sxs-lookup"><span data-stu-id="dcee8-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="dcee8-122">Cela crée le cloud, mais ne le sélectionne _pas_ automatiquement.</span><span class="sxs-lookup"><span data-stu-id="dcee8-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="dcee8-123">Si vous n’avez plus besoin du cloud créé, il peut être annulé avec la commande [cloud unregister](/cli/azure/cloud#unregister) :</span><span class="sxs-lookup"><span data-stu-id="dcee8-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

