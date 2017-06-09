---
title: Se connecter avec Azure CLI 2.0
description: Se connecter avec Azure CLI 2.0 sur Linux, Mac ou Windows.
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2017
---
# <a name="log-in-with-azure-cli-20"></a>Se connecter avec Azure CLI 2.0

Il existe plusieurs manières de se connecter et de s’authentifier auprès d’Azure CLI. Le plus simple est de vous connecter de manière interactive par l’intermédiaire de votre navigateur, ou de vous connecter à la ligne de commande. Nous vous recommandons d’utiliser des principaux du service, qui offrent un moyen de créer des comptes non interactifs que vous pouvez utiliser pour manipuler les ressources. En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir que vos scripts d’automatisation sont encore plus sûrs.

Les commandes que vous exécutez avec l’interface de ligne de commande sont exécutées sur votre abonnement par défaut.  Si vous avez plusieurs abonnements, vous souhaiterez peut-être [confirmer votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md) et le changer en conséquence.

## <a name="interactive-log-in"></a>Connexion interactive

Connectez-vous de manière interactive à partir de votre navigateur web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Ligne de commande

Fournissez vos informations d’identification sur la ligne de commande.

> [!Note]
> Cette approche ne fonctionne pas avec les comptes Microsoft ou les comptes pour lesquels l’authentification à deux facteurs est activée.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>Connexion avec un principal du service

Les principaux du service sont comme des comptes d’utilisateur auxquels vous pouvez appliquer des règles à l’aide d’Azure Active Directory.
L’authentification avec un principal du service est le meilleur moyen de sécuriser l’utilisation de vos ressources Azure à partir de vos applications ou scripts qui manipulent des ressources.
Vous définissez les rôles dont vous souhaitez que vos utilisateurs disposent par l’intermédiaire de l’ensemble de commandes `az role`.
Pour en savoir plus et pour obtenir des exemples de rôles de principal du service, consultez nos [articles de référence de rôle az](https://docs.microsoft.com/cli/azure/role.md).

1. Si vous n’avez pas encore de principal du service, [créez-en un](create-an-azure-service-principal-azure-cli.md).

1. Connectez-vous avec un principal du service.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   Pour obtenir votre locataire, connectez-vous de manière interactive, puis obtenez l’ID de locataire de votre abonnement.

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```