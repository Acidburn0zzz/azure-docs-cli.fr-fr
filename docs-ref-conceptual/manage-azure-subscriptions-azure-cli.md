---
title: Gérer des abonnements Azure avec Azure CLI
description: Gérez des abonnements Azure avec Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 27f094b68812cb68a6a33a6977d4fd58e4178731
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593657"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="19537-103">Utilisez plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="19537-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="19537-104">La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="19537-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="19537-105">Toutefois, si vous faites partie de plus d’une organisation, ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure.</span><span class="sxs-lookup"><span data-stu-id="19537-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="19537-106">L’interface CLI prend en charge la sélection d’un abonnement à la fois au niveau global et par commande.</span><span class="sxs-lookup"><span data-stu-id="19537-106">The CLI supports selecting a subscription both globally and per command.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="19537-107">Locataires, utilisateurs et abonnements</span><span class="sxs-lookup"><span data-stu-id="19537-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="19537-108">La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion.</span><span class="sxs-lookup"><span data-stu-id="19537-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="19537-109">Un _locataire_ correspond à l’entité d’Azure Active Directory qui inclut une organisation complète.</span><span class="sxs-lookup"><span data-stu-id="19537-109">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="19537-110">Ce locataire possède au moins un _abonnement_ et _utilisateur_.</span><span class="sxs-lookup"><span data-stu-id="19537-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="19537-111">Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient.</span><span class="sxs-lookup"><span data-stu-id="19537-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="19537-112">Les utilisateurs correspondent aux comptes qui se connectent à Azure afin de configurer, de gérer et d’utiliser des ressources.</span><span class="sxs-lookup"><span data-stu-id="19537-112">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="19537-113">Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure.</span><span class="sxs-lookup"><span data-stu-id="19537-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="19537-114">Chaque ressource est associée à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="19537-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="19537-115">Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="19537-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="19537-116">Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="19537-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="19537-117">Pour savoir comment se connecter à un client en particulier, consultez la rubrique [Se connecter avec Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="19537-117">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="19537-118">Modifier l’abonnement actif</span><span class="sxs-lookup"><span data-stu-id="19537-118">Change the active subscription</span></span> 

<span data-ttu-id="19537-119">Pour accéder aux ressources dédiées à un abonnement, vous devez changer votre abonnement actif, ou bien utiliser l’argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="19537-119">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="19537-120">Le changement de votre abonnement pour toutes les commandes s’effectue avec [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="19537-120">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="19537-121">Pour changer votre abonnement actif :</span><span class="sxs-lookup"><span data-stu-id="19537-121">To switch your active subscription:</span></span>

1. <span data-ttu-id="19537-122">Obtenez une liste de vos abonnements à l’aide de la commande [az account list](/cli/azure/account#az-account-list) :</span><span class="sxs-lookup"><span data-stu-id="19537-122">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="19537-123">Utilisez `az account set` avec l’ID d’abonnement ou le nom avec lequel vous souhaitez effectuer le changement.</span><span class="sxs-lookup"><span data-stu-id="19537-123">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="19537-124">Pour exécuter une seule commande avec un autre abonnement, utilisez l’argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="19537-124">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="19537-125">Cet argument accepte soit un ID d’abonnement, soit un nom d’abonnement :</span><span class="sxs-lookup"><span data-stu-id="19537-125">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
