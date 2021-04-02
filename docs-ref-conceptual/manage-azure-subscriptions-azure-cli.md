---
title: Gérer des abonnements Azure avec Azure CLI
description: Découvrez les locataires, les utilisateurs et les abonnements Azure. Utilisez Azure CLI pour gérer vos abonnements, créer des groupes d’administration et verrouiller des abonnements.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: a2a4467bc25fb8da8ced0c7b8cb6c4db9eb35e64
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581833"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a>Utiliser des abonnements Azure avec Azure CLI

Vous avez peut-être plusieurs abonnements dans Azure. Soit vous faites partie de plusieurs organisations, soit votre organisation divise l’accès à certaines ressources selon des groupes. Azure CLI prend en charge la sélection d’un abonnement à la fois au niveau global et par commande.

Pour plus d’informations sur les abonnements, la facturation et la gestion des coûts, consultez la [documentation sur la facturation et la gestion des coûts](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Locataires, utilisateurs et abonnements

Un _locataire_ correspond à l’entité d’Azure Active Directory qui inclut une organisation complète. Un locataire a un ou plusieurs _abonnements_ et _utilisateurs_. Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient. Les utilisateurs correspondent aux comptes qui se connectent à Azure afin de configurer, de gérer et d’utiliser des ressources. Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure. Chaque ressource est associée à un abonnement.

* Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).
* Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Associer ou ajouter un abonnement Azure à votre locataire Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
* Pour savoir comment se connecter à un locataire en particulier, consultez [Se connecter avec Azure CLI](./authenticate-azure-cli.md).

## <a name="commands-in-a-subscription"></a>Commandes dans un abonnement

De nombreuses commandes Azure CLI agissent au sein d’un abonnement. Vous pouvez toujours spécifier dans quel abonnement agir à l’aide du paramètre **subscription** dans votre commande. Ce paramètre est facultatif. Si vous ne spécifiez pas d’abonnement, la commande utilise votre abonnement actuel et actif.

Pour voir l’abonnement que vous êtes en train d’utiliser, exécutez la commande [az account show](/cli/azure/account#az_account_show) :

```azurecli
az account show --output table
```

> [!TIP]
> Le paramètre `--output` est un paramètre global, disponible pour toutes les commandes. La valeur **table** présente la sortie dans un format convivial. Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).

Les abonnements contiennent des groupes de ressources. Un groupe de ressources Azure est un conteneur réunissant les ressources associées d’une solution Azure. Si votre commande utilisent des ressources contenues dans votre abonnement actif, vous n’avez pas besoin de spécifier `--subscription`.

Cette commande crée un compte de stockage dans le groupe de ressources spécifié :

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

Si le groupe de stockage ne fait pas partie de votre abonnement actif actuel, cette commande échoue.

Si nécessaire, modifiez l’abonnement actif, comme décrit dans la section suivante, ou bien spécifiez l’abonnement dans la commande :

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a>Modifier l’abonnement actif

Vous pouvez modifier votre abonnement actif à l’aide de la commande [az account set](/cli/azure/account#az_account_set).

Obtenez une liste de vos abonnements à l’aide de la commande [az account list](/cli/azure/account#az_account_list) :

```azurecli
az account list --output table
```

Cette commande liste tous les abonnements auxquels vous pouvez accéder. Votre abonnement actif est marqué comme `True` dans la colonne `IsDefault`. Si, contre toute attente, il manque un abonnement, ajoutez le paramètre `--refresh` pour obtenir la liste la plus récente des abonnements.

Pour basculer vers un autre abonnement, utilisez [az account set](/cli/azure/account#az_account_set) avec l’ID ou le nom de l’abonnement vers lequel vous voulez basculer.

```azurecli
az account set --subscription "My Demos"
```

Vos abonnements ont à la fois un nom et un ID, qui est un GUID. Vous pouvez utiliser l’un ou l’autre pour ces commandes. Si vous utilisez un nom qui comprend des espaces, utilisez des guillemets.

Si vous réexécutez la commande [az account list](/cli/azure/account#az_account_list), la colonne `IsDefault` indique votre abonnement actif actuel.

## <a name="create-management-groups"></a>Créer des groupes d’administration

Les groupes d’administration Azure contiennent des abonnements. Les groupes d’administration offrent un moyen de gérer l’accès, les stratégies et la conformité de ces abonnements. Pour plus d’informations, consultez [Présentation des groupes d’administration Azure](/azure/governance/management-groups/overview).

Utilisez les commandes [az account management-group](/cli/azure/account/management-group) pour créer et gérer des groupes d’administration Azure.

Vous pouvez créer un groupe d’administration pour plusieurs de vos abonnements à l’aide de la commande [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) :

```azurecli
az account management-group create --name Contoso01
```

Pour afficher tous vos groupes d’administration, utilisez la commande [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) :

```azurecli
az account management-group list
```

Ajoutez des abonnements à votre nouveau groupe en utilisant la commande [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) :

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

Pour supprimer un abonnement, utilisez la commande [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) :

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

Pour supprimer un groupe d’administration, exécutez la commande [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) :

```azurecli
az account management-group delete --name Contoso01
```

La suppression d’un abonnement ou d’un groupe d’administration n’entraîne pas la suppression définitive ni la désactivation de cet abonnement.

## <a name="set-a-subscription-lock"></a>Définir un verrou d’abonnement

En tant qu’administrateur, vous pouvez avoir besoin de verrouiller un abonnement pour empêcher des utilisateurs de le supprimer ou de le modifier. Pour plus d’informations, consultez [Verrouiller les ressources pour empêcher les modifications inattendues](/azure/azure-resource-manager/management/lock-resources).

Dans Azure CLI, utilisez les commandes [az account lock](/cli/azure/account/lock). Par exemple, la commande [az account lock create](/cli/azure/account/lock#az_account_lock_create) peut empêcher les utilisateurs de supprimer un abonnement :

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> Vous avez besoin des autorisations appropriées pour créer ou modifier des verrous.

Pour afficher les verrous actuellement définis sur votre abonnement, utilisez la commande [az account lock list](/cli/azure/account/lock#az_account_lock_list) :

```azurecli
az account lock list --output table
```

Si vous définissez un compte en tant que compte en lecture seule, cela revient à attribuer les autorisations du rôle Lecteur à tous les utilisateurs. Pour en savoir plus sur la définition d’autorisations pour des utilisateurs individuels et des rôles, consultez [Ajouter ou supprimer des attributions de rôle Azure à l’aide d’Azure CLI](/azure/role-based-access-control/role-assignments-cli).

Pour afficher les détails d’un verrou, utilisez la commande [az account lock show](/cli/azure/account/lock#az_account_lock_show) :

```azurecli
az account lock show --name "Cannot delete subscription"
```

Vous pouvez supprimer un verrou à l’aide de la commande [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) :

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a>Voir aussi

* [Dictionnaire de la terminologie cloud Azure](/azure/azure-glossary-cloud-terminology)
* [Associer ou ajouter un abonnement Azure à votre locataire Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [Se connecter avec Azure CLI](./authenticate-azure-cli.md)
