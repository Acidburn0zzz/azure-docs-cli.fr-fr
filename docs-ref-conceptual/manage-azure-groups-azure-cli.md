---
title: Gérer les groupes de ressources Azure avec Azure CLI
description: Découvrez les groupes de ressources Azure et l’utilisation d’Azure CLI pour gérer vos groupes de ressources. Découvrez les groupes de ressources persistants et par défaut.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496076"
---
# <a name="working-with-resource-groups-in-azure-cli"></a>Utilisation de groupes de ressources dans Azure CLI

Un groupe de ressources Azure est un conteneur réunissant les ressources associées d’une solution Azure. Un groupe de ressources peut contenir du stockage, des machines virtuelles, des applications, des tableaux de bord, des services, soit presque tout ce à quoi vous avez affaire dans Azure.

## <a name="create-a-resource-group"></a>Créer un groupe de ressources

Pour créer un groupe de ressources, utilisez la commande [az group create](/cli/azure/group#az_group_create) :

```azurecli
az group create --name MyResourceGroup --location eastus
```

Un groupe de ressources appartient à un seul emplacement. Pour voir tous les emplacements pris en charge dans votre abonnement actuel, exécutez la commande [az account list-locations](/cli/azure/account#az_account_list_locations) :

```azurecli
az account list-locations
```

Pour voir tous les groupes de ressources de votre abonnement actuel, utilisez la commande [az group list](/cli/azure/group#az_group_list) :

```azurecli
az group list --output table
```

> [!TIP]
> Le paramètre `--output` est un paramètre global, disponible pour toutes les commandes. La valeur **table** présente la sortie dans un format convivial. Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).

Quand vous créez une ressource, vous la créez dans un groupe de ressources. L’exemple suivant montre un compte de stockage créé à l’aide de la commande [az storage account create](/cli/azure/storage/account#az_storage_account_create) :

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

Pour supprimer un groupe de ressources, exécutez la commande [az group delete](/cli/azure/group#az_group_delete) :

```azurecli
az group delete --name MyResourceGroup
```

Quand vous supprimez un groupe de ressources, vous supprimez toutes les ressources qui lui appartiennent. Aucune option ne permet d’annuler la suppression des ressources. Si vous essayez l’une des commandes mentionnées dans cet article, la suppression des groupes de ressources que vous créez nettoie votre compte.

## <a name="persist-a-resource-group"></a>Rendre persistant un groupe de ressources

La persistance des paramètres vous permet de réutiliser des valeurs pour certains paramètres, notamment des groupes de ressources.

Tout d’abord, activez la fonctionnalité de persistance à l’aide de la commande [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) :

```azurecli
az config param-persist on
```

Une fois la persistance activée, créez un autre groupe de ressources :

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

Tant que la persistance est activée, vous pouvez laisser le paramètre `--resource-group` hors des commandes ultérieures. La commande suivante crée un compte de stockage dans le groupe **OtherResourceGroup** :

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Si vous spécifiez un groupe de ressources dans la commande, il est prioritaire. La commande suivante crée un groupe de stockage dans un groupe de ressources appelé **StorageGroups** :

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

En revanche, une fois que vous spécifiez un autre groupe de ressources en tant que valeur, Azure CLI redéfinit la valeur rendue persistante. Les nouvelles commandes utilisent **StorageGroups** en tant que groupe de ressources. Vous pouvez afficher les valeurs rendues persistantes à l’aide de la commande [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) :

```azurecli
az config param-persist show
```

Cette commande vous montre les valeurs actuellement rendues persistantes. Ces valeurs sont stockées dans un fichier appelé *local_context_\<username>* dans un répertoire masqué appelé *.azure*. Azure CLI crée le répertoire à votre emplacement actuel quand vous créez une première valeur persistante.

Quand vous avez terminé d’utiliser des paramètres persistants, exécutez la commande [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) :

```azurecli
az config param-persist off
```

Azure CLI enregistre vos valeurs persistantes. Vous pouvez les voir dans le fichier de contexte local. Si vous réactivez la persistance des paramètres, ces valeurs sont déjà définies.

Pour plus d’informations sur l’utilisation des commandes [az config param-persist](/cli/azure/config/param-persist), consultez [Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles](/cli/azure/param-persist-tutorial).

## <a name="set-a-default-resource-group"></a>Définir un groupe de ressources par défaut

Vous pouvez définir un groupe de ressources par défaut pour toutes les commandes que vous exécutez à partir de votre Azure CLI local ou d’Azure Cloud Shell. Azure CLI stocke cette configuration localement dans un fichier *config*. Pour afficher votre configuration actuelle, exécutez la commande [az config get](/cli/azure/config#az_config_get) :

```azurecli
az config get
```

Le résultat présente les groupes de ressources par défaut et d’autres valeurs par défaut. Si vous utilisez Azure CLI pour la première fois, les résultats risquent d’être vides.

Pour définir un groupe de ressources par défaut pour votre installation Azure CLI, exécutez la commande [az config set](/cli/azure/config#az_config_set) :

```azurecli
az config set defaults.group=MyResourceGroup
```

La commande définit une valeur pour une clé spécifiée, dans cet exemple `defaults.group`. Pour connaître les options de configuration disponibles, consultez [Configuration d’Azure CLI](/cli/azure/azure-cli-configuration).

> [!NOTE]
> La commande [az config set](/cli/azure/config#az_config_set) ne valide pas l’existence du groupe de ressources que vous entrez. La commande stocke simplement la paire clé-valeur.

Une fois que vous avez exécuté la commande, les deux commandes suivantes donnent le même résultat :

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

Un groupe de ressources appartient à un abonnement. Si votre organisation a plusieurs abonnements, vous devez définir l’abonnement d’un groupe de ressources avant de l’utiliser. Si la valeur par défaut d’un groupe de ressources ne correspond pas à votre abonnement actuel, une erreur se produit. Pour plus d’informations sur les abonnements multiples, consultez [Utiliser plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md).

Vous n’avez pas besoin de réinitialiser la valeur par défaut pour utiliser d’autres groupes de ressources. Il vous suffit plutôt de spécifier le groupe de ressources :

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

La valeur par défaut est pour vous seulement. Elle n’affecte pas les autres utilisateurs ni les modifications que vous apportez par le biais du portail Azure.

Si vous utilisez des valeurs de paramètre persistantes, comme décrit dans cet article, ces valeurs sont prioritaires par rapport aux valeurs par défaut définies dans le fichier *config*.

## <a name="clean-up-resources"></a>Nettoyer les ressources

Si vous avez essayé l’une des commandes mentionnées dans cet article, vous pouvez supprimer toutes les ressources que vous avez créées en utilisant la commande [az group delete](/cli/azure/group#az_group_delete) :

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

Cette commande supprime le groupe et toutes les ressources qu’il contient en une seule opération.

Vous pouvez supprimer les paramètres persistants en exécutant la commande [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) :

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a>Voir aussi

[Configuration d’Azure CLI](/cli/azure/azure-cli-configuration)

[Tutoriel : Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles](/cli/azure/param-persist-tutorial)

[Utilisez plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md)
