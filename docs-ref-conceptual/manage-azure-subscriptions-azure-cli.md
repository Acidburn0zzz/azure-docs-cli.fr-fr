---
title: Gérer les abonnements Azure avec Azure CLI
description: Gérez les abonnements Azure avec Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: fdc8ffca38a6a581ae63b0518df72f6e09110d07
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262707"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="908d5-103">Gérer plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="908d5-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="908d5-104">La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="908d5-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="908d5-105">Toutefois, si vous faites partie de plusieurs organisations ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure.</span><span class="sxs-lookup"><span data-stu-id="908d5-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="908d5-106">Plusieurs abonnements peuvent être facilement gérés avec l’interface CLI, soit en définissant un abonnement global pour toutes les commandes, ou en sélectionnant un abonnement sur une base par commande.</span><span class="sxs-lookup"><span data-stu-id="908d5-106">Multiple subscriptions can be easily managed with the CLI either by setting a global subscription for all commands, or selecting a subscription on a per-command basis.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="908d5-107">Locataires, utilisateurs et abonnements</span><span class="sxs-lookup"><span data-stu-id="908d5-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="908d5-108">La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion.</span><span class="sxs-lookup"><span data-stu-id="908d5-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="908d5-109">Un _locataire_ est l’entité d’Azure Active Directory qui comprend une organisation complète.</span><span class="sxs-lookup"><span data-stu-id="908d5-109">A _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="908d5-110">Ce locataire possède au moins un _abonnement_ et _utilisateur_.</span><span class="sxs-lookup"><span data-stu-id="908d5-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="908d5-111">Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient.</span><span class="sxs-lookup"><span data-stu-id="908d5-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="908d5-112">Les utilisateurs sont les comptes qui se connectent à Azure pour configurer et utiliser les ressources.</span><span class="sxs-lookup"><span data-stu-id="908d5-112">Users are those accounts which log in to Azure to provision and use resources.</span></span>
<span data-ttu-id="908d5-113">Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure.</span><span class="sxs-lookup"><span data-stu-id="908d5-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="908d5-114">Chaque ressource est associée à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="908d5-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="908d5-115">Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="908d5-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="908d5-116">Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="908d5-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="908d5-117">Si vous travaillez avec plusieurs locataires, vous devrez peut-être vous connecter à un locataire spécifique.</span><span class="sxs-lookup"><span data-stu-id="908d5-117">When working with multiple tenants, you may need to sign in to a specific tenant.</span></span> <span data-ttu-id="908d5-118">Pour ce faire, consultez [Se connecter avec Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="908d5-118">To do this, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="work-with-multiple-subscriptions"></a><span data-ttu-id="908d5-119">Utilisation de plusieurs abonnements</span><span class="sxs-lookup"><span data-stu-id="908d5-119">Work with multiple subscriptions</span></span>

<span data-ttu-id="908d5-120">Pour accéder aux ressources contenues dans un abonnement, vous devez basculer vers votre abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="908d5-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="908d5-121">Un basculement de votre abonnement peut être effectué pour toutes les commandes Azure CLI avec [az account set](/cli/azure/account#az-account-set), ou par commande à l’aide de l’argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="908d5-121">Switching your subscription can be done for all Azure CLI commands with [az account set](/cli/azure/account#az-account-set), or done on a per-command basis by using the `--subscription` argument.</span></span>

<span data-ttu-id="908d5-122">Pour commencer, vous avec besoin d’une liste de vos abonnements disponibles.</span><span class="sxs-lookup"><span data-stu-id="908d5-122">To start, you will need a list of your available subscriptions.</span></span> <span data-ttu-id="908d5-123">Pour l’obtenir, utilisez la commande [az account list](/cli/azure/account#az-account-list) :</span><span class="sxs-lookup"><span data-stu-id="908d5-123">To get it, use the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli-interactive
az account list --output table
```

<span data-ttu-id="908d5-124">Pour modifier l’abonnement actif au niveau global, utilisez `az account set` avec l’ID d’abonnement ou le nom de l’abonnement :</span><span class="sxs-lookup"><span data-stu-id="908d5-124">To change the active subscription globally, use `az account set` along with either the subscription ID or subscription name:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="908d5-125">Pour utiliser un abonnement spécifique pour une commande, utilisez simplement l’argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="908d5-125">To use a specific subscription for a command, just use the `--subscription` argument.</span></span> <span data-ttu-id="908d5-126">Cet argument accepte soit un ID d’abonnement, soit un nom d’abonnement :</span><span class="sxs-lookup"><span data-stu-id="908d5-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
