---
title: Gérer des abonnements Azure avec Azure CLI
description: Gérez des abonnements Azure avec Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.product: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4c196b8376b0044e315cfee2b3958f2f4b476df7
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158321"
---
# <a name="use-multiple-azure-subscriptions"></a>Utilisez plusieurs abonnements Azure

La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement. Toutefois, si vous faites partie de plus d’une organisation, ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure. L’interface CLI prend en charge la sélection d’un abonnement à la fois au niveau global et par commande.

## <a name="tenants-users-and-subscriptions"></a>Locataires, utilisateurs et abonnements

La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion. Un _locataire_ correspond à l’entité d’Azure Active Directory qui inclut une organisation complète. Ce locataire possède au moins un _abonnement_ et _utilisateur_. Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient. Les utilisateurs correspondent aux comptes qui se connectent à Azure afin de configurer, de gérer et d’utiliser des ressources.
Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure. Chaque ressource est associée à un abonnement.

Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).  Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
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
