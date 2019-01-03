---
title: Sélectionnez des clouds avec Azure CLI
description: Créez, connectez-vous et gérez plusieurs clouds avec Azure CLI.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: e62523ba310f071020f0d66042e39e6f1867c56b
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593844"
---
# <a name="select-clouds-with-the-azure-cli"></a>Sélectionnez des clouds avec Azure CLI 

Si vous travaillez sur différentes régions ou utilisez [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), vous devrez peut-être utiliser plusieurs clouds. Microsoft fournit des clouds conformes aux lois régionales, qui sont à votre disposition. Cet article vous explique comment obtenir des informations sur les clouds, modifier le cloud actuel, et inscrire ou désinscrire de nouveaux clouds.

## <a name="list-available-clouds"></a>Répertorier les clouds disponibles

Vous pouvez lister les clouds disponibles avec la commande [az cloud list](/cli/azure/cloud#az-cloud-list). Cette commande indique quel cloud est actuellement actif, quel est son profil actuel, et elle fournit des informations concernant les noms d’hôte et les suffixes régionaux.

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

```json
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

## <a name="switch-the-active-cloud"></a>Changer de cloud actif

Pour changer le cloud actuellement actif, exécutez la commande [az cloud set](/cli/azure/cloud#az-cloud-set). Cette commande accepte un argument obligatoire, qui est le nom du cloud.

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si l’authentification pour le cloud activé a expiré, vous devez vous authentifier de nouveau avant d’effectuer d’autres tâches CLI. S’il s’agit de la première fois que vous changez vers le nouveau cloud, vous devez également configurer l’abonnement actif.
> Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md). Pour plus d’informations sur la gestion des abonnements, consultez [Gestion des abonnements Azure avec Azure CLI](manage-azure-subscriptions-azure-cli.md)

## <a name="register-a-new-cloud"></a>Inscrire un nouveau cloud

Inscrivez un nouveau cloud si vous disposez de vos propres points de terminaison pour Azure Stack. La création d’un cloud s’effectue avec la commande [az cloud register](/cli/azure/cloud#az-cloud-register). Cette commande nécessite un nom et un ensemble de points de terminaison de service. Pour savoir comment inscrire un cloud pour utilisation avec Azure Stack, consultez [Utiliser des profils de version d’API avec Azure CLI dans Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

Vous n’avez pas besoin d’inscrire votre propre cloud pour les régions de la Chine, du gouvernement des États-Unis ou de l’Allemagne. Ces clouds sont gérés par Microsoft et disponibles par défaut.  Pour plus d’informations sur tous les paramètres de point de terminaison disponibles, consultez la [documentation pour `az cloud register`](/cli/azure/cloud#az-cloud-register).

L’inscription d’un cloud n’active pas automatiquement ce dernier. Utilisez la commande `az cloud set` pour sélectionner le cloud récemment créé.

## <a name="update-an-existing-cloud"></a>Mettre à jour un cloud existant

Si vous disposez des autorisations, vous pouvez également mettre à jour un cloud existant. La mise à jour d’un cloud bascule vers un profil de services Azure différent, ou modifie les points de terminaison de connexion.
Mettez à jour un cloud avec la commande [az cloud update](/cli/azure/cloud#az-cloud-update), qui accepte les mêmes arguments que `az cloud register`.

## <a name="unregister-a-cloud"></a>Désinscrire un cloud

Si vous n’avez plus besoin du cloud créé, il peut être désinscrit avec la commande [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) :

```azurecli-interactive
az cloud unregister --name MyCloud
```
