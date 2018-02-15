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
# <a name="manage-multiple-azure-subscriptions"></a>Gérer plusieurs abonnements Azure

La plupart des utilisateurs Azure ne possèdent qu’un seul abonnement. Toutefois, si vous faites partie de plusieurs organisations ou si votre organisation a divisé l’accès à certaines ressources dans les regroupements, vous pouvez avoir plusieurs abonnements dans Azure. Il est facile de gérer plusieurs abonnements avec l’interface CLI et les opérations peuvent être effectuées en sélectionnant un abonnement.

## <a name="tenants-users-and-subscriptions"></a>Locataires, utilisateurs et abonnements

La différence entre les locataires, les utilisateurs et les abonnements dans Azure peut prêter à confusion. En règle générale, un _locataire_ est l’entité d’Azure Active Directory qui comprend une organisation complète. Ce locataire possède au moins un _abonnement_ et _utilisateur_. Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient. Les utilisateurs sont les comptes qui se connectent à Azure pour configurer et utiliser les ressources. Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure. Chaque ressource est associée à un abonnement.

Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).
Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Comment ajouter un abonnement Azure à Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).

## <a name="working-with-multiple-subscriptions"></a>Utilisation de plusieurs abonnements

Pour accéder aux ressources contenues dans un abonnement, vous devez basculer vers votre abonnement actif. Toute utilisation d’abonnements s’effectue via la commande `az account`, qui fait référence au contrat de service qu’un abonnement représente, et pas à votre compte individuel.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

Pour commencer à utiliser vos abonnements disponibles, obtenez une liste de ceux qui sont disponibles dans votre compte :

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

Pour modifier l’abonnement actif, vous pouvez utiliser `az account set` :

```azurecli-interactive
az account set --subscription "My Demos"
```

Vous pouvez utiliser l’ID ou le nom de l’abonnement pour le sélectionner.
