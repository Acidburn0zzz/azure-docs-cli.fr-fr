---
title: Utilisez des principaux du service Azure avec Azure CLI
description: Découvrez comment créer et utiliser des principaux du service avec l’interface de ligne de commande Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/15/2019
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 0969b89895ffba0ff473a9d788360609524813df
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913577"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a>Créez un principal du service avec Azure CLI

Les outils automatisés qui utilisent les services Azure doivent toujours avoir des autorisations restreintes. Plutôt que de faire se connecter des applications en tant qu’utilisateur entièrement privilégié, Azure offre des principaux du service.

Un principal de service Azure est une identité créée pour une utilisation avec les applications, des services hébergés et des outils automatisés permettant d’accéder aux ressources Azure. Cet accès est limité par les rôles assignés au principal du service, ce qui vous permet de contrôler quelles ressources sont accessibles et à quel niveau. Pour des raisons de sécurité, il est toujours recommandé d’utiliser les principaux du service avec des outils automatisés, plutôt que de leur permettre de se connecter avec une identité d’utilisateur.

Cet article vous explique les étapes à suivre pour créer, réinitialiser et obtenir des informations sur un principal du service avec l’interface de ligne de commande Azure.

## <a name="create-a-service-principal"></a>Créer un principal du service

Créez un principal de service à l’aide de la commande [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac). Lorsque vous créez un principal de service, vous choisissez le type d’authentification de connexion qu’il utilise. 

> [!NOTE]
>
> Si votre compte ne dispose pas d’autorisations pour créer un principal de service, `az ad sp create-for-rbac` vous retournera un message d’erreur contenant « Privilèges insuffisants pour effectuer l’opération ». Contactez votre administrateur Azure Active Directory pour créer un principal de service.

Il existe deux types d’authentification disponibles pour les principaux de service : L’authentification basée sur un mot de passe et l’authentification basée sur un certificat.

### <a name="password-based-authentication"></a>L’authentification basée sur un mot de passe

Sans aucun paramètre d’authentification, l’authentification basée sur un mot de passe est utilisée avec un mot de passe aléatoire créé pour vous.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> À compter d’Azure CLI 2.0.68, le paramètre `--password` permettant de créer un principal de service avec un mot de passe défini par l’utilisateur __n’est plus pris en charge__ pour empêcher l’utilisation accidentelle de mots de passe faibles.

La sortie d’un principal de service avec l’authentification par mot de passe comprend la clé `password`. __Assurez-vous__ d’avoir copié cette valeur : elle ne pourra être récupérée. Si vous oubliez le mot de passe, effectuez une [réinitialisation des informations d’identification du principal du service](#reset-credentials).

Les clés `appId` et `tenant` s’affichent dans la sortie de `az ad sp create-for-rbac` et sont utilisés dans l’authentification du principal du service.
Enregistrez leurs valeurs, mais elles peuvent être récupérées à tout moment avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list).

### <a name="certificate-based-authentication"></a>Authentification par certificat

Pour l’authentification basée sur un certificat, utilisez l’argument `--cert`. Cet argument requiert que vous possédiez un certificat existant. Assurez-vous que n’importe quel outil qui utilise ce principal de service a accès à la clé privée du certificat. Les certificats doivent être au format ASCII tel que PEM, CER ou DER. Transmettez le certificat sous forme de chaîne, ou utilisez le format `@path` pour charger le certificat depuis un fichier.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

L’argument `--keyvault` peut être ajouté pour utiliser un certificat dans Azure Key Vault. Dans ce cas, la valeur `--cert` fait référence au nom du certificat.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

Pour créer un certificat _auto-signé_ pour l’authentification, utilisez l’argument `--create-cert` :

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

L’argument `--keyvault` peut être ajouté pour stocker le certificat dans Azure Key Vault. Lorsque vous utilisez `--keyvault`, l’argument `--cert` est __requis__.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

À moins que vous ne stockiez le certificat dans Key Vault, la sortie comprend la clé `fileWithCertAndPrivateKey`. La valeur de cette clé vous indique l’emplacement dans lequel le certificat généré est stocké.
__Assurez-vous__ d’avoir copié le certificat à un emplacement sécurisé ou vous ne pourrez pas vous connecter avec ce principal de service.

Pour les certificats stockés dans Key Vault, récupérez la clé privée du certificat avec l’[affichage du secret du coffre de clés az](/cli/azure/keyvault/secret#az-keyvault-secret-show). Dans Key Vault, le nom du secret du certificat est le même que le nom du certificat. Si vous perdez l’accès à la clé privée d’un certificat, effectuez la [réinitialisation des informations d’identification du principal du service](#reset-credentials).

Les clés `appId` et `tenant` s’affichent dans la sortie de `az ad sp create-for-rbac` et sont utilisés dans l’authentification du principal du service.
Enregistrez leurs valeurs, mais elles peuvent être récupérées à tout moment avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list).

## <a name="get-an-existing-service-principal"></a>Obtenir un principal de service existant

Une liste des principaux de service dans un locataire peut être récupérée avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list). Par défaut, la commande retourne les cents premiers principaux de service de votre locataire. Pour obtenir tous les principaux de service d’un locataire, utilisez l’argument `--all`. Obtenir cette liste peut prendre beaucoup de temps, il est donc recommandé de filtrer la liste avec l’un des arguments suivants :

* `--display-name` demande les principaux de service ayant un _préfixe_ qui correspond au nom fourni. Le nom d’affichage d’un principal de service est la valeur définie avec le paramètre `--name` lors de la création. Si vous n’avez pas défini `--name` lors de la création du principal de service, le nom du préfixe est `azure-cli-`.
* `--spn` filtre la correspondance exacte de nom de principal du service. Le nom de principal du service commence toujours par `https://`.
  si la valeur que vous avez utilisé pour `--name` n’était pas un URI, cette valeur est `https://` suivie du nom d’affichage.
* `--show-mine` demande uniquement les principaux du service créés par l’utilisateur connecté.
* `--filter` utilise un filtre OData et effectue un filtrage _côté serveur_. Cette méthode est préférable au filtrage côté client avec l’argument `--query` de l’interface de ligne de commande. Pour en savoir plus sur les filtres OData, consultez [syntaxe d’expression de filtres OData](/rest/api/searchservice/odata-expression-syntax-for-azure-search).

Les informations retournées pour les objets de principaux du service sont détaillées. Pour obtenir uniquement les informations nécessaires pour vous connecter, utilisez la chaîne de requête `[].{id:appId, tenant:appOwnerTenantId}`. Par exemple, pour obtenir les informations de connexion de tous les principaux du service créés par l’utilisateur actuellement connecté :

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> `az ad sp list` ou [affichage az ad sp](/cli/azure/ad/sp#az-ad-sp-show) permettent d’obtenir l’utilisateur et le locataire, mais pas les secrets d’authentification _ou_ la méthode d’authentification.
> Les secrets des certificats dans Key Vault peuvent être récupérés avec [affichage du secret du coffre de clés az](/cli/azure/keyvault/secret#az-keyvault-secret-show), mais aucun autre secret n’est stocké par défaut.
> Si vous oubliez une méthode d’authentification ou un secret, effectuez la [réinitialisation des informations d’identification du principal du service](#reset-credentials).

## <a name="manage-service-principal-roles"></a>Gérer les rôles du principal du service

L’interface de ligne de commande Azure fournit les commandes suivantes de gestion d’attributions de rôle :

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

Un principal du service a le rôle **Contributor** (Collaborateur) par défaut. Ce rôle dispose des autorisations complètes de lecture et d’écriture dans un compte Azure. Le rôle de **Lecteur** est plus restrictif avec un accès en lecture seule.  Pour plus d’informations sur les rôles et le contrôle d’accès en fonction du rôle, consultez [RBAC : rôles intégrés pour les ressources Azure](/azure/active-directory/role-based-access-built-in-roles).

Cet exemple ajoute le rôle de **Lecteur** et supprime le rôle de **Contributeur** :

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> Si votre compte ne dispose pas d’autorisations pour assigner un rôle, un message d’erreur vous indiquera que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ ». Contactez votre administrateur Azure Active Directory pour gérer les rôles.

L’ajout d’un rôle ne restreint _pas_ les autorisations précédemment assignées. Lors de la restriction des autorisations du principal du service, le rôle de __Contributeur__ dot être supprimé.

Les modifications peuvent être vérifiées en répertoriant les rôles attribués :

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a>Se connecter en tant que principal du service

Testez les informations d’identification et les autorisations du nouveau principal du service en vous connectant. Pour vous connecter avec un principal du service, vous avez besoin de `appId`, `tenant` ainsi que des informations d’identification.

Pour vous connecter avec un principal du service utilisant un mot de passe :

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Pour vous connecter avec un certificat, celui-ci doit être disponible localement sous forme de fichier PEM ou DER, ou au format ASCII :

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

Pour en savoir plus sur la connexion avec un principal du service, consultez [Se connecter avec l’interface de ligne de commande Azure](authenticate-azure-cli.md).

## <a name="reset-credentials"></a>Réinitialiser les informations d’identification

Si vous avez oublié les informations d’identification d’un principal du service, utilisez la [réinitialisation des informations d’identification az ad sp](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). La commande de réinitialisation utilise les mêmes arguments que `az ad sp create-for-rbac`.

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
