---
title: "Créer un principal du service avec Azure CLI 2.0"
description: "Découvrez comment créer un principal du service pour votre application ou service avec Azure CLI 2.0."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 10/12/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: a6ad5611f3e507b65e160122c87e22ec44546588
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/18/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Créer un principal du service avec Azure CLI 2.0

Si vous prévoyez de gérer votre application ou service avec Azure CLI 2.0, vous devez l’exécuter sous un principal du service Azure Active Directory (AAD) plutôt que vos propres informations d’identification.
Cette rubrique vous guide tout au long de la création d’une entité de sécurité avec Azure CLI 2.0.

> [!NOTE]
> Vous pouvez également créer un principal du service par l’intermédiaire du portail Azure.
> Pour plus d’informations, consultez [Utiliser le portail pour créer une application et un principal du service Active Directory pouvant accéder aux ressources](/azure/azure-resource-manager/resource-group-create-service-principal-portal).

## <a name="what-is-a-service-principal"></a>Qu’est-ce qu’un « principal du service » ?

Un principal du service Azure est une identité de sécurité utilisée par les applications, les services et les outils d’automatisation créés par l’utilisateur pour accéder à des ressources Azure spécifiques. Il équivaut un peu à une identité d’utilisateur (connexion et mot de passe ou certificat) avec un rôle spécifique et des autorisations d’accès à vos ressources étroitement contrôlées. Il doit pouvoir effectuer uniquement des opérations spécifiques, contrairement à une identité d’utilisateur. Il améliore la sécurité si vous lui octroyez seulement le niveau d’autorisation minimal nécessaire pour effectuer ses tâches de gestion. 

Azure CLI 2.0 prend en charge la création d’informations d’authentification basées sur un mot de passe et d’informations d’identification de certificat. Dans cette rubrique, nous traitons les deux types d’informations d’identification.

## <a name="verify-your-own-permission-level"></a>Vérifier votre propre niveau d’autorisation

Tout d’abord, vous devez avoir les autorisations suffisantes dans votre annuaire Azure Active Directory et votre abonnement Azure. Plus précisément, vous devez pouvoir créer une application dans l’annuaire Active Directory et affecter un rôle au principal du service. 

Le moyen le plus simple pour vérifier que votre compte dispose des autorisations adéquates est d’utiliser le portail. Consultez [Vérifier l’autorisation requise dans le portail](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).

## <a name="create-a-service-principal-for-your-application"></a>Créer un principal du service pour votre application

Vous devez disposer de l’un des éléments suivants pour identifier l’application pour laquelle vous souhaitez créer un principal du service :

  * Le nom unique ou l’URI de votre application déployée (par exemple, « MyDemoWebApp » dans les exemples), ou
  * L’ID d’application, le GUID unique associé à votre application, service ou objet déployé

Ces valeurs identifient votre application lors de la création d’un principal du service.

### <a name="get-information-about-your-application"></a>Obtenir des informations sur votre application

Obtenez des informations sur l’identité de votre application avec la commande `az ad app list`.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

L’option `--display-name` filtre la liste des applications retournées pour afficher celles dont le `displayName` commence par MyDemoWebApp.

### <a name="create-a-service-principal-with-a-password"></a>Créer un principal du service avec un mot de passe

Utilisez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) et le paramètre `--password` pour créer le principal du service avec un mot de passe. Lorsque vous ne fournissez pas de rôle ou d’étendue, le rôle **Contributeur** est défini par défaut pour l’abonnement actuel. Si vous créez un principal du service sans utiliser les paramètres `--password` ou `--cert`, l’authentification par mot de passe est employée et un mot de passe est généré.

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
``` 

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING] 
 > Ne créez pas un mot de passe non sécurisé.  Suivez les conseils en matière de [Stratégies et restrictions de mot de passe dans Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).

### <a name="create-a-service-principal-with-a-self-signed-certificate"></a>Créer un principal du service avec un certificat auto-signé

Utilisez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) et le paramètre `--create-cert` pour créer un certificat auto-signé.

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --create-cert
```

```json
{
  "appId": "c495db57-82e0-4e2e-9369-069dff176858",
  "displayName": "azure-cli-2017-10-12-22-15-38",
  "fileWithCertAndPrivateKey": "<path>/<file-name>.pem",
  "name": "http://MyDemoWebApp",
  "password": null,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Copiez la valeur de la réponse `fileWithCertAndPrivateKey`. Il s’agit du fichier de certificat qui sera utilisé pour l’authentification.

Pour plus d’options lors de l’utilisation de certificats, consultez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).

### <a name="get-information-about-the-service-principal"></a>Obtenir des informations sur le principal du service

```azurecli-interactive
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a>Se connecter en tant que principal du service

Vous pouvez à présent vous connecter en tant que nouveau principal du service pour votre application à l’aide de l’*appId* de `az ad sp show` et du *mot de passe* ou du chemin d’accès au certificat créé.  Fournissez la valeur *tenant* indiquée dans les résultats de `az ad sp create-for-rbac`.

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password-or-path-to-cert} --tenant {tenant}
``` 

Après une ouverture de session réussie, la sortie suivante s’affiche :

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

Utilisez les valeurs `id`, `password` et `tenant` comme informations d’identification pour exécuter votre application. 

## <a name="managing-roles"></a>Gestion des rôles 

> [!NOTE]
> Le contrôle d’accès en fonction du rôle (RBAC) dans Azure est un modèle utilisé pour définir et gérer les rôles des principaux de l’utilisateur et du service.
> Les rôles sont associés à des ensembles d’autorisations, qui déterminent les ressources qu’un principal peut lire, écrire ou gérer, ou auxquelles il peut accéder.
> Pour plus d’informations sur le contrôle d’accès en fonction du rôle et les rôles, consultez [Rôles intégrés pour le contrôle d’accès en fonction du rôle Azure](/azure/active-directory/role-based-access-built-in-roles).

Azure CLI 2.0 fournit les commandes suivantes pour gérer les attributions de rôle :

* [az role assignment list](/cli/azure/role/assignment#list)
* [az role assignment create](/cli/azure/role/assignment#create)
* [az role assignment delete](/cli/azure/role/assignment#delete)

Le rôle par défaut pour un principal du service est **Contributor**. Il ne s’agit pas nécessairement du meilleur choix pour les interactions d’une application avec les services Azure, étant donné ses autorisations étendues. Le rôle **Reader** est plus restrictif et constitue un bon choix pour l’accès en lecture seule. Vous pouvez afficher des détails sur les autorisations propres à un rôle ou créer des autorisations personnalisées par l’intermédiaire du portail Azure.

Dans cet exemple, ajoutez le rôle **Reader** à notre exemple précédent, puis supprimez le rôle **Contributor** :

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

Vérifiez les modifications apportées en énumérant les rôles actuellement affectés :

```azurecli-interactive
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE] 
> Si votre compte ne dispose pas des autorisations suffisantes pour affecter un rôle, un message d’erreur s’affiche.
> Le message indique que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ sur l’étendue ’/subscriptions/{guid}’ ».
   
## <a name="change-the-credentials-of-a-security-principal"></a>Changer les informations d’identification d’une entité de sécurité

Nous vous recommandons de passer en revue les autorisations et de mettre régulièrement à jour les mots de passe. Vous pouvez également gérer et modifier les informations d’identification de sécurité à mesure que votre application change.

### <a name="reset-a-service-principal-password"></a>Réinitialiser un mot de passe de principal du service

Utilisez `az ad sp reset-credentials` pour réinitialiser le mot de passe actuel du principal du service.

```azurecli-interactive
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

L’interface de ligne de commande génère un mot de passe sécurisé si vous omettez l’option `--password`.
