---
title: "Gérer les abonnements Azure avec Azure CLI 2.0"
description: "Gérer les abonnements Azure avec Azure CLI 2.0 sur Linux, Mac ou Windows."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 9f03e52fa72a8dbd5753904839a833db01ffb59b
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="d4fb3-103">Gérer plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="d4fb3-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="d4fb3-104">La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="d4fb3-105">Toutefois, si vous faites partie de plusieurs organisations ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="d4fb3-106">Il est facile de gérer plusieurs abonnements avec l’interface CLI et les opérations peuvent être effectuées en sélectionnant un abonnement.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="d4fb3-107">Locataires, utilisateurs et abonnements</span><span class="sxs-lookup"><span data-stu-id="d4fb3-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="d4fb3-108">La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="d4fb3-109">En règle générale, un _locataire_ est l’entité d’Azure Active Directory qui comprend une organisation complète.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="d4fb3-110">Ce locataire possède au moins un _abonnement_ et _utilisateur_.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="d4fb3-111">Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="d4fb3-112">Les utilisateurs sont les comptes qui se connectent à Azure pour configurer et utiliser les ressources.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="d4fb3-113">Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="d4fb3-114">Chaque ressource est associée à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="d4fb3-115">Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="d4fb3-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="d4fb3-116">Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="d4fb3-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="d4fb3-117">Utilisation de plusieurs abonnements</span><span class="sxs-lookup"><span data-stu-id="d4fb3-117">Working with multiple subscriptions</span></span>

<span data-ttu-id="d4fb3-118">Pour accéder aux ressources contenues dans un abonnement, vous devez basculer vers votre abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-118">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="d4fb3-119">Toute utilisation d’abonnements s’effectue via la commande `az account`, qui fait référence au contrat de service qu’un abonnement représente, et pas à votre compte individuel.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-119">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="d4fb3-120">Pour commencer à utiliser vos abonnements disponibles, obtenez une liste de ceux qui sont disponibles dans votre compte :</span><span class="sxs-lookup"><span data-stu-id="d4fb3-120">To start working with your available subscriptions, get a list of those available in your account:</span></span>

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

<span data-ttu-id="d4fb3-121">Pour modifier l’abonnement actif, vous pouvez utiliser `az account set` :</span><span class="sxs-lookup"><span data-stu-id="d4fb3-121">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="d4fb3-122">Vous pouvez utiliser l’ID ou le nom de l’abonnement pour le sélectionner.</span><span class="sxs-lookup"><span data-stu-id="d4fb3-122">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
