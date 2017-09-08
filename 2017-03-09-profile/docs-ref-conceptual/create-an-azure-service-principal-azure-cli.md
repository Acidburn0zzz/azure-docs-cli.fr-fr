---
title: "Créer un principal du service avec Azure CLI 2.0"
description: "Découvrez comment créer un principal du service pour votre application ou service avec Azure CLI 2.0."
keywords: Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: f37df762a9a605ea649b215f38f2e9866614f4ac
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="e2630-104">Créer un principal du service avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e2630-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="e2630-105">Si vous prévoyez de gérer votre application ou service avec Azure CLI 2.0, vous devez l’exécuter sous un principal du service Azure Active Directory (AAD) plutôt que vos propres informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="e2630-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="e2630-106">Cette rubrique vous guide tout au long de la création d’une entité de sécurité avec Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="e2630-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="e2630-107">Vous pouvez également créer un principal du service par l’intermédiaire du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="e2630-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="e2630-108">Pour plus d’informations, consultez [Utiliser le portail pour créer une application et un principal du service Active Directory pouvant accéder aux ressources](/azure/azure-resource-manager/resource-group-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="e2630-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="e2630-109">Qu’est-ce qu’un « principal du service » ?</span><span class="sxs-lookup"><span data-stu-id="e2630-109">What is a 'service principal'?</span></span>

<span data-ttu-id="e2630-110">Un principal du service Azure est une identité de sécurité utilisée par les applications, les services et les outils d’automatisation créés par l’utilisateur pour accéder à des ressources Azure spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e2630-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="e2630-111">Il équivaut un peu à une identité d’utilisateur (connexion et mot de passe ou certificat) avec un rôle spécifique et des autorisations d’accès à vos ressources étroitement contrôlées.</span><span class="sxs-lookup"><span data-stu-id="e2630-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="e2630-112">Il doit pouvoir effectuer uniquement des opérations spécifiques, contrairement à une identité d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e2630-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="e2630-113">Il améliore la sécurité si vous lui octroyez seulement le niveau d’autorisation minimal nécessaire pour effectuer ses tâches de gestion.</span><span class="sxs-lookup"><span data-stu-id="e2630-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="e2630-114">À l’heure actuelle, Azure CLI 2.0 prend en charge uniquement la création d’informations d’identification d’authentification basées sur mot de passe.</span><span class="sxs-lookup"><span data-stu-id="e2630-114">Right now, Azure CLI 2.0 only supports the creation of password-based authentication credentials.</span></span> <span data-ttu-id="e2630-115">Dans cette rubrique, nous abordons la création d’un principal du service avec un mot de passe spécifique et l’affectation éventuelle de rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e2630-115">In this topic, we cover creating a service principal with a specific password, and optionally assigning specific roles to it.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="e2630-116">Vérifier votre propre niveau d’autorisation</span><span class="sxs-lookup"><span data-stu-id="e2630-116">Verify your own permission level</span></span>

<span data-ttu-id="e2630-117">Tout d’abord, vous devez avoir les autorisations suffisantes dans votre annuaire Azure Active Directory et votre abonnement Azure.</span><span class="sxs-lookup"><span data-stu-id="e2630-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="e2630-118">Plus précisément, vous devez pouvoir créer une application dans l’annuaire Active Directory et affecter un rôle au principal du service.</span><span class="sxs-lookup"><span data-stu-id="e2630-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="e2630-119">Le moyen le plus simple pour vérifier que votre compte dispose des autorisations adéquates est d’utiliser le portail.</span><span class="sxs-lookup"><span data-stu-id="e2630-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="e2630-120">Consultez [Vérifier l’autorisation requise dans le portail](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="e2630-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="e2630-121">Créer un principal du service pour votre application</span><span class="sxs-lookup"><span data-stu-id="e2630-121">Create a service principal for your application</span></span>

<span data-ttu-id="e2630-122">Vous devez disposer de l’un des éléments suivants pour identifier l’application pour laquelle vous souhaitez créer un principal du service :</span><span class="sxs-lookup"><span data-stu-id="e2630-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="e2630-123">Le nom unique ou l’URI de votre application déployée (par exemple, « MyDemoWebApp » dans les exemples), ou</span><span class="sxs-lookup"><span data-stu-id="e2630-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="e2630-124">L’ID d’application, le GUID unique associé à votre application, service ou objet déployé</span><span class="sxs-lookup"><span data-stu-id="e2630-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="e2630-125">Ces valeurs identifient votre application lors de la création d’un principal du service.</span><span class="sxs-lookup"><span data-stu-id="e2630-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="e2630-126">Obtenir des informations sur votre application</span><span class="sxs-lookup"><span data-stu-id="e2630-126">Get information about your application</span></span>

<span data-ttu-id="e2630-127">Obtenez des informations sur l’identité de votre application avec la commande `az ad app list`.</span><span class="sxs-lookup"><span data-stu-id="e2630-127">Get identity information about your application with the `az ad app list`.</span></span>

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

<span data-ttu-id="e2630-128">L’option `--display-name` filtre la liste des applications retournées pour afficher celles dont le `displayName` commence par MyDemoWebApp.</span><span class="sxs-lookup"><span data-stu-id="e2630-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-the-service-principal"></a><span data-ttu-id="e2630-129">Créer le principal du service</span><span class="sxs-lookup"><span data-stu-id="e2630-129">Create the service principal</span></span>

<span data-ttu-id="e2630-130">Utilisez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) pour créer le principal du service.</span><span class="sxs-lookup"><span data-stu-id="e2630-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) to create the service principal.</span></span> 

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
 > <span data-ttu-id="e2630-131">Ne créez pas un mot de passe non sécurisé.</span><span class="sxs-lookup"><span data-stu-id="e2630-131">Don't create an insecure password.</span></span>  <span data-ttu-id="e2630-132">Suivez les conseils en matière de [Stratégies et restrictions de mot de passe dans Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="e2630-132">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="e2630-133">Obtenir des informations sur le principal du service</span><span class="sxs-lookup"><span data-stu-id="e2630-133">Get information about the service principal</span></span>

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

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="e2630-134">Se connecter à l’aide du principal du service</span><span class="sxs-lookup"><span data-stu-id="e2630-134">Sign in using the service principal</span></span>

<span data-ttu-id="e2630-135">Vous pouvez maintenant vous connecter en tant que nouveau principal du service pour votre application en utilisant l’*appId* et le *password* fournis par la commande `az ad sp show`.</span><span class="sxs-lookup"><span data-stu-id="e2630-135">You can now log in as the new service principal for your app using the *appId* and *password* from `az ad sp show`.</span></span>  <span data-ttu-id="e2630-136">Fournissez la valeur *tenant* indiquée dans les résultats de `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="e2630-136">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

<span data-ttu-id="e2630-137">Après une ouverture de session réussie, la sortie suivante s’affiche :</span><span class="sxs-lookup"><span data-stu-id="e2630-137">You will see this output after a successful sign-on:</span></span>

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

<span data-ttu-id="e2630-138">Utilisez les valeurs `id`, `password` et `tenant` comme informations d’identification pour exécuter votre application.</span><span class="sxs-lookup"><span data-stu-id="e2630-138">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="e2630-139">Gestion des rôles</span><span class="sxs-lookup"><span data-stu-id="e2630-139">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="e2630-140">Le contrôle d’accès en fonction du rôle (RBAC) dans Azure est un modèle utilisé pour définir et gérer les rôles des principaux de l’utilisateur et du service.</span><span class="sxs-lookup"><span data-stu-id="e2630-140">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="e2630-141">Les rôles sont associés à des ensembles d’autorisations, qui déterminent les ressources qu’un principal peut lire, écrire ou gérer, ou auxquelles il peut accéder.</span><span class="sxs-lookup"><span data-stu-id="e2630-141">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="e2630-142">Pour plus d’informations sur le contrôle d’accès en fonction du rôle et les rôles, consultez [Rôles intégrés pour le contrôle d’accès en fonction du rôle Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="e2630-142">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="e2630-143">Azure CLI 2.0 fournit les commandes suivantes pour gérer les attributions de rôle :</span><span class="sxs-lookup"><span data-stu-id="e2630-143">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="e2630-144">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="e2630-144">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="e2630-145">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="e2630-145">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="e2630-146">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="e2630-146">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="e2630-147">Le rôle par défaut pour un principal du service est **Contributor**.</span><span class="sxs-lookup"><span data-stu-id="e2630-147">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="e2630-148">Il ne s’agit pas nécessairement du meilleur choix pour les interactions d’une application avec les services Azure, étant donné ses autorisations étendues.</span><span class="sxs-lookup"><span data-stu-id="e2630-148">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="e2630-149">Le rôle **Reader** est plus restrictif et constitue un bon choix pour l’accès en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e2630-149">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="e2630-150">Vous pouvez afficher des détails sur les autorisations propres à un rôle ou créer des autorisations personnalisées par l’intermédiaire du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="e2630-150">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="e2630-151">Dans cet exemple, ajoutez le rôle **Reader** à notre exemple précédent, puis supprimez le rôle **Contributor** :</span><span class="sxs-lookup"><span data-stu-id="e2630-151">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="e2630-152">Vérifiez les modifications apportées en énumérant les rôles actuellement affectés :</span><span class="sxs-lookup"><span data-stu-id="e2630-152">Verify the changes by listing the currently assigned roles:</span></span>

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
> <span data-ttu-id="e2630-153">Si votre compte ne dispose pas des autorisations suffisantes pour affecter un rôle, un message d’erreur s’affiche.</span><span class="sxs-lookup"><span data-stu-id="e2630-153">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="e2630-154">Le message indique que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ sur l’étendue ’/subscriptions/{guid}’ ».</span><span class="sxs-lookup"><span data-stu-id="e2630-154">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="e2630-155">Changer les informations d’identification d’une entité de sécurité</span><span class="sxs-lookup"><span data-stu-id="e2630-155">Change the credentials of a security principal</span></span>

<span data-ttu-id="e2630-156">Nous vous recommandons de passer en revue les autorisations et de mettre régulièrement à jour les mots de passe.</span><span class="sxs-lookup"><span data-stu-id="e2630-156">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="e2630-157">Vous pouvez également gérer et modifier les informations d’identification de sécurité à mesure que votre application change.</span><span class="sxs-lookup"><span data-stu-id="e2630-157">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="e2630-158">Réinitialiser un mot de passe de principal du service</span><span class="sxs-lookup"><span data-stu-id="e2630-158">Reset a service principal password</span></span>

<span data-ttu-id="e2630-159">Utilisez `az ad sp reset-credentials` pour réinitialiser le mot de passe actuel du principal du service.</span><span class="sxs-lookup"><span data-stu-id="e2630-159">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

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

<span data-ttu-id="e2630-160">L’interface de ligne de commande génère un mot de passe sécurisé si vous omettez l’option `--password`.</span><span class="sxs-lookup"><span data-stu-id="e2630-160">The CLI generates a secure password if you leave out the `--password` option.</span></span>
