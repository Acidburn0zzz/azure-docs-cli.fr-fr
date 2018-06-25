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
# <a name="manage-multiple-azure-subscriptions"></a>Gérer plusieurs abonnements Azure

La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement. Toutefois, si vous faites partie de plusieurs organisations ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure. Plusieurs abonnements peuvent être facilement gérés avec l’interface CLI, soit en définissant un abonnement global pour toutes les commandes, ou en sélectionnant un abonnement sur une base par commande.

## <a name="tenants-users-and-subscriptions"></a>Locataires, utilisateurs et abonnements

La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion. Un _locataire_ est l’entité d’Azure Active Directory qui comprend une organisation complète. Ce locataire possède au moins un _abonnement_ et _utilisateur_. Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient. Les utilisateurs sont les comptes qui se connectent à Azure pour configurer et utiliser les ressources.
Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure. Chaque ressource est associée à un abonnement.

Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).  Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Si vous travaillez avec plusieurs locataires, vous devrez peut-être vous connecter à un locataire spécifique. Pour ce faire, consultez [Se connecter avec Azure CLI](/cli/azure/authenticate-azure-cli).

## <a name="work-with-multiple-subscriptions"></a>Utilisation de plusieurs abonnements

Pour accéder aux ressources contenues dans un abonnement, vous devez basculer vers votre abonnement actif. Un basculement de votre abonnement peut être effectué pour toutes les commandes Azure CLI avec [az account set](/cli/azure/account#az-account-set), ou par commande à l’aide de l’argument `--subscription`.

Pour commencer, vous avec besoin d’une liste de vos abonnements disponibles. Pour l’obtenir, utilisez la commande [az account list](/cli/azure/account#az-account-list) :

```azurecli-interactive
az account list --output table
```

Pour modifier l’abonnement actif au niveau global, utilisez `az account set` avec l’ID d’abonnement ou le nom de l’abonnement :

```azurecli-interactive
az account set --subscription "My Demos"
```

Pour utiliser un abonnement spécifique pour une commande, utilisez simplement l’argument `--subscription`. Cet argument accepte soit un ID d’abonnement, soit un nom d’abonnement :

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
