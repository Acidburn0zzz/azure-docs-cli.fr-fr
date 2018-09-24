---
title: Se connecter avec Azure CLI 2.0
description: Se connecter avec Azure CLI 2.0 de façon interactive avec des informations d’identification locales
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: f6f3e8bc015420795dda48da093bc92bbf246529
ms.sourcegitcommit: 8e6e3129f8f4824a8acfa12edb5dae52466d4be8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2018
ms.locfileid: "45626922"
---
# <a name="sign-in-with-azure-cli-20"></a>Se connecter avec Azure CLI 2.0

Il existe plusieurs types d’authentification pour l’interface Azure CLI. Le moyen le plus simple pour commencer est d’utiliser [Azure Cloud Shell](/azure/cloud-shell/overview), qui vous connecte automatiquement. Localement, vous pouvez vous connecter de manière interactive via votre navigateur avec la commande `az login`. Lors de l’écriture de scripts, l’approche recommandée consiste à utiliser des principaux du service. En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir la sécurité de votre automatisation.

Aucune de vos informations de connexion n’est stockée par l’interface CLI. Au lieu de cela, un [jeton d’actualisation d’authentification](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-id-and-access-tokens#refresh-tokens) est généré par Azure, puis stocké. Depuis août 2018, ce jeton est révoqué après 90 jours d’inactivité, mais cette valeur peut être modifiée par Microsoft ou votre administrateur client. Une fois le jeton révoqué, vous recevez un message de l’interface CLI indiquant que vous devez vous reconnecter.

Une fois connecté, les commandes CLI sont exécutées sur votre abonnement par défaut. Si vous possédez plusieurs abonnements, vous pouvez [modifier votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Connexion interactive

La méthode d’authentification par défaut Azure CLI utilise un navigateur web et un jeton d’accès pour la connexion.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Connectez-vous à l’aide de vos informations d’identification sur la ligne de commande

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

Vous pouvez sélectionner un locataire pour vous connecter avec l’argument `--tenant`. La valeur de cet argument peut être un domaine `.onmicrosoft.com`, ou l’ID d’objet Azure du locataire. Les méthodes de connexion interactive et avec une ligne de commande fonctionnent toutes les deux avec `--tenant`.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Connexion avec un principal de service

Les principaux de service sont des comptes non liés à un utilisateur spécifique, qui peuvent détenir des autorisations sur ces derniers par le biais de rôles prédéfinis. L’authentification avec un principal de service est la meilleure façon d’écrire des scripts ou des programmes sécurisés, ce qui vous permet d’appliquer des restrictions d’autorisation et des informations d’identification statiques stockées localement. Pour en savoir plus sur les principaux de service, consultez [Créer un principal du service avec Azure CLI](create-an-azure-service-principal-azure-cli.md).

Pour vous connecter avec un principal de service, il vous faut :

* L’URL ou le nom associé au principal du service
* Le mot de passe du principal de service ou le certificat X509 utilisé pour créer le principal du service au format PEM
* Le locataire associé au principal du service, comme un domaine `.onmicrosoft.com` ou un ID d’objet Azure

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
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
