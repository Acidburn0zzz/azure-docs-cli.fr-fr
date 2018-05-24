---
title: La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0
description: Créer, se connecter et gérer plusieurs clouds avec l’interface de ligne de commande Azure 2.0.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7ccee3a336f4c596f29783a70ba0cd4398e20b95
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/18/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0

Si vous travaillez sur différentes régions ou utilisez [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), vous devrez peut-être utiliser plusieurs clouds. Microsoft fournit des clouds conformes aux lois régionales, qui sont à votre disposition. Cet article explique comment obtenir des informations sur les clouds disponibles sur votre compte, modifier le cloud actuel, et inscrire ou annuler désinscrire nouveaux clouds à utiliser avec Azure Stack.

## <a name="listing-clouds"></a>Énumération des clouds

Vous pouvez lister les clouds disponibles avec la commande [az cloud list](/cli/azure/cloud#az-cloud-list). Elle indique quel cloud est actuellement actif, son profil actuel, et fournit des informations sur les noms d’hôte et les suffixes régionaux.

Pour obtenir le cloud actif et une liste de tous les clouds disponibles :

```azurecli-interactive
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

Le cloud actuellement actif a `True` dans la colonne `IsActive`. Un seul cloud peut être actif à tout moment. Pour obtenir des informations plus détaillées sur un cloud, y compris sur les points de terminaison qu’il utilise pour les services Azure, utilisez la commande `cloud show` :

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switching-the-active-cloud"></a>Changement du cloud actif

Pour changer le cloud actuellement actif, exécutez la commande [az cloud set](/cli/azure/cloud#az-cloud-set). Cette commande accepte un argument obligatoire, qui est le nom du cloud.

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si l’authentification pour le cloud activé a expiré, vous devez vous authentifier de nouveau avant d’effectuer d’autres tâches CLI. S’il s’agit de la première fois que vous changez vers le nouveau cloud, vous devez également configurer l’abonnement actif.
> Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec l’interface de ligne de commande Azure 2.0](authenticate-azure-cli.md). Pour plus d’informations sur la gestion des abonnements, consultez [Gestion des abonnements Azure avec Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-cloud"></a>Inscrire un cloud

Inscrivez un nouveau cloud si vous disposez de vos propres points de terminaison pour Azure Stack. La création d’un cloud s’effectue avec la commande [az cloud register](/cli/azure/cloud#az-cloud-register). Cette commande nécessite un nom et un ensemble de fonctionnalités avec les points de terminaison associés. Pour savoir comment inscrire un cloud pour une utilisation avec Azure Stack, consultez [Utiliser des profils de version des API avec Azure CLI 2.0 dans Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

Vous n’avez pas besoin d’inscrire votre propre cloud pour les régions de la Chine, du Gouvernement des États-Unis ou de l’Allemagne. Celles-ci sont gérées par Microsoft et disponibles par défaut.  Pour plus d’informations sur tous les paramètres de point de terminaison disponibles, consultez la [documentation pour `az cloud register`](/cli/azure/cloud#az-cloud-register).

L’inscription d’un cloud n’active pas automatiquement ce dernier. Utilisez la commande `az cloud set` pour sélectionner le cloud qui vient d’être créé comme décrit ci-dessus.

## <a name="update-an-existing-cloud"></a>Mettre à jour un cloud existant

Si vous disposez des autorisations, vous pouvez également mettre à jour un cloud existant. Faites-le lorsque vous avez besoin de basculer vers un autre profil Azure, ou d’ajouter ou de modifier un point de terminaison.
Faites-le avec la commande [az cloud update](/cli/azure/cloud#az-cloud-update), qui accepte les mêmes arguments que `az cloud register`.

## <a name="unregister-a-cloud"></a>Désinscrire un cloud

Si vous n’avez plus besoin d’un cloud inscrit, vous pouvez le désinscrire avec la commande [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) :

```azurecli-interactive
az cloud unregister --name MyCloud
```
