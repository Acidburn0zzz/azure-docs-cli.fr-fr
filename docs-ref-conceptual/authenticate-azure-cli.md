---
title: Se connecter avec Azure CLI 2.0
description: "Se connecter avec Azure CLI 2.0 de façon interactive avec des informations d’identification locales"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 92c96b7e969de686689ef02bf068392b9f565698
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2018
---
# <a name="log-in-with-azure-cli-20"></a>Se connecter avec Azure CLI 2.0

Il existe plusieurs manières de se connecter et de s’authentifier auprès d’Azure CLI. Le plus simple est de vous connecter de manière interactive par l’intermédiaire de votre navigateur, via Azure Cloud Shell ou la commande `az login`.
L’approche recommandée consiste à utiliser des principaux du service, qui sont des comptes à autorisations restreintes. En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir que vos scripts d’automatisation sont encore plus sûrs.

Aucune des informations d’identification privées n’est stockée localement. Au lieu de cela, un jeton d’authentification est généré par Azure, puis stocké. Une fois connecté, votre jeton de connexion est valide jusqu’à 14 jours sans être utilisé. Au-delà, vous devez vous authentifier de nouveau.

Une fois connecté, les commandes CLI sont exécutées sur votre abonnement par défaut. Si vous avez plusieurs abonnements, vous pouvez [modifier votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Connexion interactive

Connectez-vous de manière interactive à partir de votre navigateur web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Ligne de commande

Fournissez vos informations d’identification sur la ligne de commande.

> [!Note]
> Cette approche ne fonctionne pas avec les comptes Microsoft ou les comptes pour lesquels l’authentification à deux facteurs est activée.

```azurecli
az login -u <username> -p <password>
```

## <a name="log-in-with-a-specific-tenant"></a>Se connecter avec un locataire spécifique

Si vous travaillez avec plusieurs locataires, vous pouvez sélectionner le locataire auquel vous connecter avec l’argument `--tenant`. La valeur de cet argument peut être un domaine `.onmicrosoft.com`, ou l’ID d’objet Azure du locataire. Vous pouvez vous connecter de manière interactive, ou fournir vos informations d’identification avec les arguments `--user` et `--password`. 

```
az login --tenant <tenant>
```

## <a name="logging-in-with-a-service-principal"></a>Connexion avec un principal du service

Les principaux de service sont des comptes non liés à un utilisateur spécifique, qui peuvent détenir des autorisations sur ces derniers par le biais de rôles prédéfinis. L’authentification avec un principal de service est la meilleure façon d’écrire des scripts ou des programmes sécurisés, ce qui vous permet d’appliquer des restrictions d’autorisation et des informations d’identification statiques stockées localement. Pour en savoir plus sur les principaux de service, consultez [Créer un principal du service avec Azure CLI](create-an-azure-service-principal-azure-cli.md).

Pour vous connecter avec un principal du service, renseignez le nom d’utilisateur, le mot de passe ou fichier de certificat PEM, et le locataire associé au principal du service :

```azurecli
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

La valeur du locataire est le locataire Azure Active Directory associé au principal du service. Il peut s’agir d’un domaine `.onmicrosoft.com`, ou de l’ID d’objet Azure du locataire.
Vous pouvez obtenir l’ID objet du locataire pour votre connexion actuelle à l’aide de la commande suivante :

```azurecli
az account show --query 'tenantId' -o tsv
```
