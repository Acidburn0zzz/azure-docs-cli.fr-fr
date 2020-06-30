---
title: Gérer des abonnements Azure avec Azure CLI
description: Gérez des abonnements Azure avec Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 2c5f81b53806d0c7d8de7e48b8214f4ccd65c154
ms.sourcegitcommit: 5c3a54d7e9153a67f9caaf0d2415f6d9c297ebee
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/16/2020
ms.locfileid: "84819611"
---
# <a name="use-multiple-azure-subscriptions"></a>Utilisez plusieurs abonnements Azure

La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement. Toutefois, si vous faites partie de plus d’une organisation, ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure. L’interface CLI prend en charge la sélection d’un abonnement à la fois au niveau global et par commande.

Pour plus d’informations sur les abonnements, la facturation et la gestion des coûts, consultez la [documentation sur la facturation et la gestion des coûts](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Locataires, utilisateurs et abonnements

La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion. Un _locataire_ correspond à l’entité d’Azure Active Directory qui inclut une organisation complète. Ce locataire possède au moins un _abonnement_ et _utilisateur_. Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient. Les utilisateurs correspondent aux comptes qui se connectent à Azure afin de configurer, de gérer et d’utiliser des ressources.
Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure. Chaque ressource est associée à un abonnement.

Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).  Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Associer ou ajouter un abonnement Azure à votre locataire Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Pour savoir comment se connecter à un client en particulier, consultez la rubrique [Se connecter avec Azure CLI](/cli/azure/authenticate-azure-cli).

## <a name="change-the-active-subscription"></a>Modifier l’abonnement actif

Pour accéder aux ressources dédiées à un abonnement, vous devez changer votre abonnement actif, ou bien utiliser l’argument `--subscription`. Le changement de votre abonnement pour toutes les commandes s’effectue avec [az account set](/cli/azure/account#az-account-set).

Pour changer votre abonnement actif :

1. Obtenez une liste de vos abonnements à l’aide de la commande [az account list](/cli/azure/account#az-account-list) :

    ```azurecli-interactive
    az account list --output table
    ```
2. Utilisez `az account set` avec l’ID d’abonnement ou le nom avec lequel vous souhaitez effectuer le changement.

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

Pour exécuter une seule commande avec un autre abonnement, utilisez l’argument `--subscription`. Cet argument accepte soit un ID d’abonnement, soit un nom d’abonnement :

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
