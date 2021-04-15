---
title: Créer une demande de support Azure dans Azure CLI
description: Découvrez comment utiliser les commandes de support az Azure CLI pour créer, mettre à jour et gérer les demandes de support Azure.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to, devx-track-azurecli
ms.openlocfilehash: 45387d352d94dcc044861e540932b38b954a16be
ms.sourcegitcommit: bff138c7d3cd3ce8c90c5809b0e812be71959504
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/14/2021
ms.locfileid: "107385788"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a><span data-ttu-id="e4ea6-103">Créer une demande de support Azure dans Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e4ea6-103">Create an Azure support request in Azure CLI</span></span>

<span data-ttu-id="e4ea6-104">L’interface Azure CLI vous permet de créer et de gérer des tickets de support Azure.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-104">The Azure CLI enables you to create and manage Azure support tickets.</span></span>

- <span data-ttu-id="e4ea6-105">Ouvrir un ticket de support technique, de facturation, d’abonnement ou de gestion d’abonnement et de limites de service (quota).</span><span class="sxs-lookup"><span data-stu-id="e4ea6-105">Open a technical, billing, subscription management, or subscription and service limits (quota) support ticket.</span></span>
- <span data-ttu-id="e4ea6-106">Obtenir la liste des tickets de support et des informations détaillées sur chaque ticket.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-106">Get a list of support tickets and detailed information about each ticket.</span></span> <span data-ttu-id="e4ea6-107">Affiner votre recherche de tickets de support par état ou date de création.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-107">Narrow your search for support tickets by status or created date.</span></span>
- <span data-ttu-id="e4ea6-108">Mettre à jour la gravité, l’état et les informations de contact d’un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-108">Update severity, ticket status, and contact information for a support ticket.</span></span>
- <span data-ttu-id="e4ea6-109">Ajouter une nouvelle communication à un ticket de support ou obtenir la liste de toutes les communications en rapport avec un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-109">Add a new communication to a support ticket or get a list of all communications for a support ticket.</span></span> <span data-ttu-id="e4ea6-110">Affiner votre recherche de listes de communication par date de création ou type de communication.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-110">Narrow your search of communication lists by created date or communication type.</span></span>

<span data-ttu-id="e4ea6-111">Pour créer une demande de support, vous devez être [Propriétaire](/azure/role-based-access-control/built-in-roles#owner) ou [Contributeur](/azure/role-based-access-control/built-in-roles#contributor) ou le rôle [Contributeur de demande de support](/azure/role-based-access-control/built-in-roles#support-request-contributor) doit vous avoir été attribuer au niveau de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-111">To create a support request, you must be an [Owner](/azure/role-based-access-control/built-in-roles#owner) or [Contributor](/azure/role-based-access-control/built-in-roles#contributor), or be assigned to the [Support Request Contributor](/azure/role-based-access-control/built-in-roles#support-request-contributor) role at the subscription level.</span></span> <span data-ttu-id="e4ea6-112">Pour créer une demande de support sans abonnement, comme dans un scénario Azure Active Directory, vous devez être [Administrateur](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ea6-112">To create a support request without a subscription, such as an Azure Active Directory scenario, you must be an [Admin](/azure/active-directory/roles/permissions-reference).</span></span>

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a><span data-ttu-id="e4ea6-113">Création d’un ticket de support</span><span class="sxs-lookup"><span data-stu-id="e4ea6-113">Create a support ticket</span></span>

1. <span data-ttu-id="e4ea6-114">Pour obtenir une liste de services, utilisez la commande [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-114">To obtain a list of services, use the [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) command:</span></span>

   ```azurecli
   az support services list --output table
   ```

   <span data-ttu-id="e4ea6-115">Pour cet exemple, recherchez la valeur de la **machine virtuelle exécutant Windows**, qui est **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-115">For this example, find the value for **Virtual Machine running Windows**, which is **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span></span>

1. <span data-ttu-id="e4ea6-116">Pour connaître le type de problème et le sous-type de problème qui décrivent votre problème, exécutez la commande [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-116">To get the problem type and problem subtype that describes your problem, run the [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) command:</span></span>

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   <span data-ttu-id="e4ea6-117">Pour cet exemple, recherchez **Impossible de me connecter à ma machine virtuelle / J’ai un problème avec mon IP publique**.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-117">For this example, find **Cannot connect to my VM / I have an issue with my public IP**.</span></span> <span data-ttu-id="e4ea6-118">Ce type a la valeur **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-118">That type has a value of **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span></span>

1. <span data-ttu-id="e4ea6-119">Créez un ticket en utilisant la commande [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-119">Create a ticket by using the [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) command:</span></span>

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

<span data-ttu-id="e4ea6-120">Un ingénieur de support vous contactera en utilisant la méthode que vous avez indiquée.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-120">A support engineer will contact you using the method you indicated.</span></span> <span data-ttu-id="e4ea6-121">Pour plus d’informations sur le temps de réponse initial, consultez [Étendue du support et réactivité](/support/plans/response/).</span><span class="sxs-lookup"><span data-stu-id="e4ea6-121">For information about initial response times, see [Support scope and responsiveness](/support/plans/response/).</span></span>

## <a name="manage-support-tickets"></a><span data-ttu-id="e4ea6-122">Gestion des tickets de support</span><span class="sxs-lookup"><span data-stu-id="e4ea6-122">Manage support tickets</span></span>

<span data-ttu-id="e4ea6-123">Pour voir vos tickets de support de votre abonnement actuel, exécutez la commande [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-123">To see your support tickets for your current subscription, run the [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) command:</span></span>

```azurecli
az support tickets list
```

<span data-ttu-id="e4ea6-124">Pour voir les tickets de support d’un autre abonnement, exécutez la commande [az account set](/cli/azure/account#az_account_set) pour changer votre abonnement actuel, puis exécutez la commande.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-124">To see support tickets in another subscription, run the [az account set](/cli/azure/account#az_account_set) command to change your current subscription, and then run the command.</span></span>

<span data-ttu-id="e4ea6-125">Vous pouvez également mettre à jour un ticket à l’aide de la commande [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-125">You can also update a ticket by using the [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) command:</span></span>

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a><span data-ttu-id="e4ea6-126">Communiquer sur votre ticket</span><span class="sxs-lookup"><span data-stu-id="e4ea6-126">Communicate about your ticket</span></span>

<span data-ttu-id="e4ea6-127">Vous ne pouvez pas supprimer un ticket de support créé avec Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-127">You can't delete a support ticket created by using Azure CLI.</span></span> <span data-ttu-id="e4ea6-128">À la place, envoyez un message pour fermer un ticket.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-128">Instead, send a message to close a ticket.</span></span> <span data-ttu-id="e4ea6-129">Si vous devez rouvrir une demande de support clôturée, créez un message, qui rouvre automatiquement la demande.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-129">If you need to reopen a closed support request, create a new message, which automatically reopens the request.</span></span>

<span data-ttu-id="e4ea6-130">Pour communiquer sur votre ticket, exécutez la commande [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-130">To communicate about your ticket, run the [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) command:</span></span>

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

<span data-ttu-id="e4ea6-131">Pour voir toutes les communications sur un ticket, utilisez la commande [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) :</span><span class="sxs-lookup"><span data-stu-id="e4ea6-131">To see all the communications for a ticket, use the [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) command:</span></span>

```azurecli
az support tickets communications list --ticket-name VM012
```

<span data-ttu-id="e4ea6-132">Cette commande offre un paramètre `--filters` pour affiner vos réponses.</span><span class="sxs-lookup"><span data-stu-id="e4ea6-132">This command offers a `--filters` parameter to narrow your responses.</span></span>

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a><span data-ttu-id="e4ea6-133">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e4ea6-133">Next steps</span></span>

- [<span data-ttu-id="e4ea6-134">Questions fréquentes (FAQ) sur le support technique Azure</span><span class="sxs-lookup"><span data-stu-id="e4ea6-134">Azure Support FAQs</span></span>](https://azure.microsoft.com/support/faq/)
- [<span data-ttu-id="e4ea6-135">Niveaux de gravité Azure</span><span class="sxs-lookup"><span data-stu-id="e4ea6-135">Azure severity and levels</span></span>](https://azure.microsoft.com/support/plans/response/)
- [<span data-ttu-id="e4ea6-136">Guide pratique pour créer un ticket de support via le portail Azure</span><span class="sxs-lookup"><span data-stu-id="e4ea6-136">How to create a support ticket via Azure portal</span></span>](/azure/azure-portal/supportability/how-to-create-azure-support-request)
