---
title: Utiliser des principaux du service avec Azure CLI 2.0
description: "Découvrez comment créer et utiliser un principal du service avec Azure CLI 2.0."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/12/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b46c735a14240bddd07659475ada1c33c75a1e67
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Créer un principal du service avec Azure CLI 2.0

Si vous souhaitez créer une connexion distincte avec des restrictions d’accès, vous pouvez le faire via un principal du service. Les principaux de service sont des identités distinctes qui peuvent être associées à un compte. Ils sont utiles pour travailler avec des applications et des tâches devant être automatisées. Cet article vous guide tout au long du processus de création d’un principal de service.

## <a name="create-the-service-principal"></a>Créer le principal du service

Utilisez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) pour créer un principal de service. Le nom du principal du service n’est lié à aucune application ou nom d’utilisateur existant. Vous pouvez créer un principal de service avec votre choix du type d’authentification.

* `--password` est utilisé pour l’authentification par mot de passe. Vérifiez que vous créez un mot de passe fort en suivant les [règles et restrictions relatives aux mots de passe Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). Si vous ne spécifiez pas de mot de passe, un mot de passe est créé pour vous.

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* `--cert` est utilisé pour l’authentification basée sur les certificats pour un certificat existant, soit en tant que chaîne publique PEM ou DER, ou `@{file}` pour charger un fichier.

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  L’argument `--keyvault` peut être ajouté pour indiquer que le certificat est stocké dans Azure Key Vault. Dans ce cas, la valeur `--cert` fait référence au nom du certificat dans le coffre de clés.

* `--create-cert` crée un certificat _auto-signé_ pour l’authentification. L’argument `--keyvault` peut être ajouté pour stocker le certificat dans Azure Key Vault.

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

Si un argument indiquant le type d’authentification n’est pas inclus, `--password` est utilisé par défaut.

Le résultat de la commande `create-for-rbac` est au format suivant :

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Les valeurs `appId`, `tenant`, et `password` sont utilisées pour l’authentification. La valeur `displayName` est utilisée lors de la recherche d’un principal du service existant.

> [!NOTE]
> Si votre compte ne dispose pas des autorisations suffisantes pour créer un principal du service, un message d’erreur contenant « Privilèges insuffisants pour effectuer l’opération. » s’affiche. Contactez votre administrateur Azure Active Directory pour créer un principal de service.

## <a name="manage-service-principal-roles"></a>Gérer les rôles du principal du service 

Azure CLI 2.0 fournit les commandes suivantes pour gérer les attributions de rôle.

* [az role assignment list](/cli/azure/role/assignment#list)
* [az role assignment create](/cli/azure/role/assignment#create)
* [az role assignment delete](/cli/azure/role/assignment#delete)

Un principal du service a le rôle **Contributor** (Collaborateur) par défaut. Ce rôle dispose des autorisations complètes de lecture et d’écriture dans un compte Azure et n’est généralement pas approprié pour les applications. Le rôle **Reader** est plus restrictif et constitue un accès en lecture seule.  Pour plus d’informations sur le contrôle d’accès en fonction du rôle (RBAC) et les rôles, consultez [RBAC : rôles intégrés](/azure/active-directory/role-based-access-built-in-roles).

Cet exemple ajoute le rôle **Lecteur** et supprime le rôle **Contributeur**.

```azurecli
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

L’ajout d’un rôle ne modifie _pas_ les autorisations précédemment affectées. Lors de la restriction des autorisations du principal du service, le rôle __Contributeur__ rôle doit toujours être supprimé.

Les modifications peuvent être vérifiées en répertoriant les rôles attribués.

```azurecli
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> Le message indique que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ sur l’étendue ’/subscriptions/{guid}’ » lorsque votre compte ne dispose pas d’autorisations suffisantes pour affecter un rôle. Contactez votre administrateur Azure Active Directory pour gérer les rôles.

## <a name="log-in-using-the-service-principal"></a>Se connecter en tant que principal du service

Vous pouvez tester la connexion et les autorisations du principal du service en ouvrant une session sous ce dernier dans Azure CLI. Connectez-vous en tant que nouveau principal du service à l’aide de `appId`, `tenant`et des valeurs des informations d’identification. Les informations d’authentification que vous fournissez changent selon que vous avez choisi de créer le principal du service avec un mot de passe ou un certificat.

Pour vous connecter avec un mot de passe, vous devez le fournir en tant que paramètre d’argument.

```azurecli
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Pour vous connecter avec un certificat, celui-ci doit être disponible localement sous forme de fichier PEM ou DER.

```azurecli
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```
## <a name="reset-credentials"></a>Réinitialiser les informations d’identification

Si vous oubliez les informations d’identification relatives à un principal de service, il est possible de les réinitialiser à l’aide de la commande [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials). Les mêmes restrictions et options de création d’un principal de service s’appliquent également ici.

```azurecli
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
