---
title: Créer une demande de support Azure dans Azure CLI
description: Découvrez comment utiliser les commandes de support az Azure CLI pour créer, mettre à jour et gérer les demandes de support Azure.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to
ms.openlocfilehash: 297b8b65973a7d2b3d377a56865f1cbdd42e08f2
ms.sourcegitcommit: 936ec07eb1c56e24d8000cc24a2a0e05102e0cf4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "104911122"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a>Créer une demande de support Azure dans Azure CLI

L’interface Azure CLI vous permet de créer et de gérer des tickets de support Azure.

- Ouvrir un ticket de support technique, de facturation, d’abonnement ou de gestion d’abonnement et de limites de service (quota).
- Obtenir la liste des tickets de support et des informations détaillées sur chaque ticket. Affiner votre recherche de tickets de support par état ou date de création.
- Mettre à jour la gravité, l’état et les informations de contact d’un ticket de support.
- Ajouter une nouvelle communication à un ticket de support ou obtenir la liste de toutes les communications en rapport avec un ticket de support. Affiner votre recherche de listes de communication par date de création ou type de communication.

Pour créer une demande de support, vous devez être [Propriétaire](/azure/role-based-access-control/built-in-roles#owner) ou [Contributeur](/azure/role-based-access-control/built-in-roles#contributor) ou le rôle [Contributeur de demande de support](/azure/role-based-access-control/built-in-roles#support-request-contributor) doit vous avoir été attribuer au niveau de l’abonnement. Pour créer une demande de support sans abonnement, comme dans un scénario Azure Active Directory, vous devez être [Administrateur](/azure/active-directory/roles/permissions-reference).

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a>Création d’un ticket de support

1. Pour obtenir une liste de services, utilisez la commande [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) :

   ```azurecli
   az support services list --output table
   ```

   Pour cet exemple, recherchez la valeur de la **machine virtuelle exécutant Windows**, qui est **6f16735c-b0ae-b275-ad3a-03479cfa1396**.

1. Pour connaître le type de problème et le sous-type de problème qui décrivent votre problème, exécutez la commande [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) :

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   Pour cet exemple, recherchez **Impossible de me connecter à ma machine virtuelle / J’ai un problème avec mon IP publique**. Ce type a la valeur **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.

1. Créez un ticket en utilisant la commande [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) :

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

Un ingénieur de support vous contactera en utilisant la méthode que vous avez indiquée. Pour plus d’informations sur le temps de réponse initial, consultez [Étendue du support et réactivité](/support/plans/response/).

## <a name="manage-support-tickets"></a>Gestion des tickets de support

Pour voir vos tickets de support de votre abonnement actuel, exécutez la commande [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) :

```azurecli
az support tickets list
```

Pour voir les tickets de support d’un autre abonnement, exécutez la commande [az account set](/cli/azure/account#az_account_set) pour changer votre abonnement actuel, puis exécutez la commande.

Vous pouvez également mettre à jour un ticket à l’aide de la commande [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) :

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a>Communiquer sur votre ticket

Vous ne pouvez pas supprimer un ticket de support créé avec Azure CLI. À la place, envoyez un message pour fermer un ticket. Si vous devez rouvrir une demande de support clôturée, créez un message, qui rouvre automatiquement la demande.

Pour communiquer sur votre ticket, exécutez la commande [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) :

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

Pour voir toutes les communications sur un ticket, utilisez la commande [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) :

```azurecli
az support tickets communications list --ticket-name VM012
```

Cette commande offre un paramètre `--filters` pour affiner vos réponses.

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a>Étapes suivantes

- [Questions fréquentes (FAQ) sur le support technique Azure](https://azure.microsoft.com/support/faq/)
- [Niveaux de gravité Azure](https://azure.microsoft.com/support/plans/response/)
- [Guide pratique pour créer un ticket de support via le portail Azure](/azure/azure-portal/supportability/how-to-create-azure-support-request)
