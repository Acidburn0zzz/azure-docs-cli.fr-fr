---
title: Se connecter avec Azure CLI 2.0
description: Se connecter avec Azure CLI 2.0 de façon interactive avec des informations d’identification locales
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/09/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: a0e05b3306cc273486b1b5fc887ceedbf78cb779
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967756"
---
# <a name="sign-in-with-azure-cli-20"></a>Se connecter avec Azure CLI 2.0

Il existe plusieurs manières de s’authentifier auprès d’Azure CLI. Le plus simple est de vous connecter de manière interactive par l’intermédiaire de votre navigateur, via Azure Cloud Shell ou la commande `az login`.
L’approche recommandée consiste à utiliser des principaux du service, qui sont des comptes à autorisations restreintes. En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir que vos scripts d’automatisation sont encore plus sûrs.

Aucune des informations d’identification privées n’est stockée localement. Au lieu de cela, un jeton d’authentification est généré par Azure, puis stocké. Une fois connecté, votre jeton d’authentification est valide jusqu’à 14 jours sans être utilisé. Au-delà, vous devez vous authentifier de nouveau.

Une fois connecté, les commandes CLI sont exécutées sur votre abonnement par défaut. Si vous avez plusieurs abonnements, vous pouvez [modifier votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-sign-in"></a>Connexion interactive

La méthode d’authentification par défaut Azure CLI utilise un navigateur web et un jeton d’accès pour la connexion.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Ligne de commande

Fournissez vos informations d’identification d’utilisateur Azure dans la ligne de commande.

> [!Note]
> Cette approche ne fonctionne pas avec les comptes Microsoft ou les comptes pour lesquels l’authentification à deux facteurs est activée.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Si vous souhaitez éviter l’affichage de votre mot de passe sur la console et que vous utilisez `az login` de manière interactive, utilisez la commande `read -s` sous `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> Dans PowerShell, utilisez la cmdlet `Read-Host -AsSecureString` et la conversion de chaînes sécurisée.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="sign-in-with-a-specific-tenant"></a>Se connecter avec un locataire spécifique

Si vous travaillez avec plusieurs locataires, vous pouvez sélectionner le locataire auquel vous connecter avec l’argument `--tenant`. La valeur de cet argument peut être un domaine `.onmicrosoft.com`, ou l’ID d’objet Azure du locataire. Vous pouvez vous connecter de manière interactive, ou fournir vos informations d’identification avec les arguments `--user` et `--password`.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Connexion avec un principal de service

Les principaux de service sont des comptes non liés à un utilisateur spécifique, qui peuvent détenir des autorisations sur ces derniers par le biais de rôles prédéfinis. L’authentification avec un principal de service est la meilleure façon d’écrire des scripts ou des programmes sécurisés, ce qui vous permet d’appliquer des restrictions d’autorisation et des informations d’identification statiques stockées localement. Pour en savoir plus sur les principaux de service, consultez [Créer un principal du service avec Azure CLI](create-an-azure-service-principal-azure-cli.md).

Pour vous connecter avec un principal du service, renseignez le nom d’utilisateur, le mot de passe ou fichier de certificat PEM, et le locataire associé au principal du service :

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

La valeur du locataire est le locataire Azure Active Directory associé au principal du service. Il peut s’agir d’un domaine `.onmicrosoft.com`, ou de l’ID d’objet Azure du locataire.
Vous pouvez obtenir l’ID objet du locataire pour votre compte actuellement actif à l’aide de la commande suivante :

```azurecli-interactive
az account show --query 'tenantId' -o tsv
```

> [!IMPORTANT]
> Si vous souhaitez éviter l’affichage de votre mot de passe sur la console et que vous utilisez `az login` de manière interactive, utilisez la commande `read -s` sous `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> Dans PowerShell, utilisez la cmdlet `Read-Host -AsSecureString` et la conversion de chaînes sécurisée.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```
