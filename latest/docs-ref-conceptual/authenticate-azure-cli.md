---
title: Se connecter avec Azure CLI 2.0
description: Se connecter avec Azure CLI 2.0 sur Linux, Mac ou Windows.
keywords: Azure CLI 2.0, connexion, Azure CLI, authentification, autorisation, se connecter
author: sptramer
ms.author: stttramer
manager: routlaw
ms.date: 11/13/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 0a8ec3541783ae19961f2acf1192c0ee061a465f
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2017
---
# <a name="log-in-with-azure-cli-20"></a>Se connecter avec Azure CLI 2.0

Il existe plusieurs manières de se connecter et de s’authentifier auprès d’Azure CLI. Le plus simple est de vous connecter de manière interactive par l’intermédiaire de votre navigateur, ou de vous connecter à la ligne de commande. Nous vous recommandons d’utiliser des principaux du service, qui offrent un moyen de créer des comptes non interactifs que vous pouvez utiliser pour manipuler les ressources. En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir que vos scripts d’automatisation sont encore plus sûrs.

Aucune des informations d’identification privées n’est stockée localement. Au lieu de cela, un jeton d’authentification est généré par Azure, puis stocké. Une fois connecté, votre jeton de connexion locale est valide jusqu’à 14 jours sans être utilisé. Au-delà, vous devrez vous authentifier de nouveau.

Une fois connecté, les commandes CLI sont exécutées sur votre abonnement par défaut. Si vous avez plusieurs abonnements, vous souhaiterez peut-être [modifier votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md).

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
L’authentification avec un principal du service est le meilleur moyen de sécuriser l’utilisation de vos ressources Azure à partir de vos applications ou scripts qui manipulent des ressources. Si vous n’avez pas encore de principal du service disponible et que vous souhaitez en créer un, consultez [Créer un principal du service Azure avec Azure CLI](create-an-azure-service-principal-azure-cli.md).

Pour vous connecter avec un principal du service, renseignez le nom d’utilisateur, le mot de passe ou fichier de certificat PEM, et le locataire associé au principal du service :

```azurecli-interactive
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

La valeur du locataire est le locataire Azure Active Directory associé au principal du service. Il peut s’agir d’un domaine .onmicrosoft.com, ou de l’ID objet Azure du locataire.
Vous pouvez obtenir l’ID objet du locataire pour votre connexion actuelle à l’aide de la commande suivante :

```azurecli
az account show --query 'tenantId' -o tsv
```

