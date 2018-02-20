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
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="b63ae-103">Créer un principal du service avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="b63ae-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="b63ae-104">Si vous souhaitez créer une connexion distincte avec des restrictions d’accès, vous pouvez le faire via un principal du service.</span><span class="sxs-lookup"><span data-stu-id="b63ae-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="b63ae-105">Les principaux de service sont des identités distinctes qui peuvent être associées à un compte.</span><span class="sxs-lookup"><span data-stu-id="b63ae-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="b63ae-106">Ils sont utiles pour travailler avec des applications et des tâches devant être automatisées.</span><span class="sxs-lookup"><span data-stu-id="b63ae-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="b63ae-107">Cet article vous guide tout au long du processus de création d’un principal de service.</span><span class="sxs-lookup"><span data-stu-id="b63ae-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="b63ae-108">Créer le principal du service</span><span class="sxs-lookup"><span data-stu-id="b63ae-108">Create the service principal</span></span>

<span data-ttu-id="b63ae-109">Utilisez [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) pour créer un principal de service.</span><span class="sxs-lookup"><span data-stu-id="b63ae-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="b63ae-110">Le nom du principal du service n’est lié à aucune application ou nom d’utilisateur existant.</span><span class="sxs-lookup"><span data-stu-id="b63ae-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="b63ae-111">Vous pouvez créer un principal de service avec votre choix du type d’authentification.</span><span class="sxs-lookup"><span data-stu-id="b63ae-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="b63ae-112">`--password` est utilisé pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="b63ae-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="b63ae-113">Vérifiez que vous créez un mot de passe fort en suivant les [règles et restrictions relatives aux mots de passe Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="b63ae-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="b63ae-114">Si vous ne spécifiez pas de mot de passe, un mot de passe est créé pour vous.</span><span class="sxs-lookup"><span data-stu-id="b63ae-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="b63ae-115">`--cert` est utilisé pour l’authentification basée sur les certificats pour un certificat existant, soit en tant que chaîne publique PEM ou DER, ou `@{file}` pour charger un fichier.</span><span class="sxs-lookup"><span data-stu-id="b63ae-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="b63ae-116">L’argument `--keyvault` peut être ajouté pour indiquer que le certificat est stocké dans Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="b63ae-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="b63ae-117">Dans ce cas, la valeur `--cert` fait référence au nom du certificat dans le coffre de clés.</span><span class="sxs-lookup"><span data-stu-id="b63ae-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

* <span data-ttu-id="b63ae-118">`--create-cert` crée un certificat _auto-signé_ pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="b63ae-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="b63ae-119">L’argument `--keyvault` peut être ajouté pour stocker le certificat dans Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="b63ae-119">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

<span data-ttu-id="b63ae-120">Si un argument indiquant le type d’authentification n’est pas inclus, `--password` est utilisé par défaut.</span><span class="sxs-lookup"><span data-stu-id="b63ae-120">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="b63ae-121">Le résultat de la commande `create-for-rbac` est au format suivant :</span><span class="sxs-lookup"><span data-stu-id="b63ae-121">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="b63ae-122">Les valeurs `appId`, `tenant`, et `password` sont utilisées pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="b63ae-122">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="b63ae-123">La valeur `displayName` est utilisée lors de la recherche d’un principal du service existant.</span><span class="sxs-lookup"><span data-stu-id="b63ae-123">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="b63ae-124">Si votre compte ne dispose pas des autorisations suffisantes pour créer un principal du service, un message d’erreur contenant « Privilèges insuffisants pour effectuer l’opération. » s’affiche.</span><span class="sxs-lookup"><span data-stu-id="b63ae-124">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="b63ae-125">Contactez votre administrateur Azure Active Directory pour créer un principal de service.</span><span class="sxs-lookup"><span data-stu-id="b63ae-125">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="b63ae-126">Gérer les rôles du principal du service</span><span class="sxs-lookup"><span data-stu-id="b63ae-126">Manage service principal roles</span></span> 

<span data-ttu-id="b63ae-127">Azure CLI 2.0 fournit les commandes suivantes pour gérer les attributions de rôle.</span><span class="sxs-lookup"><span data-stu-id="b63ae-127">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="b63ae-128">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="b63ae-128">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="b63ae-129">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="b63ae-129">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="b63ae-130">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="b63ae-130">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="b63ae-131">Un principal du service a le rôle **Contributor** (Collaborateur) par défaut.</span><span class="sxs-lookup"><span data-stu-id="b63ae-131">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="b63ae-132">Ce rôle dispose des autorisations complètes de lecture et d’écriture dans un compte Azure et n’est généralement pas approprié pour les applications.</span><span class="sxs-lookup"><span data-stu-id="b63ae-132">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="b63ae-133">Le rôle **Reader** est plus restrictif et constitue un accès en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="b63ae-133">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="b63ae-134">Pour plus d’informations sur le contrôle d’accès en fonction du rôle (RBAC) et les rôles, consultez [RBAC : rôles intégrés](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="b63ae-134">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="b63ae-135">Cet exemple ajoute le rôle **Lecteur** et supprime le rôle **Contributeur**.</span><span class="sxs-lookup"><span data-stu-id="b63ae-135">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="b63ae-136">L’ajout d’un rôle ne modifie _pas_ les autorisations précédemment affectées.</span><span class="sxs-lookup"><span data-stu-id="b63ae-136">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="b63ae-137">Lors de la restriction des autorisations du principal du service, le rôle __Contributeur__ rôle doit toujours être supprimé.</span><span class="sxs-lookup"><span data-stu-id="b63ae-137">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="b63ae-138">Les modifications peuvent être vérifiées en répertoriant les rôles attribués.</span><span class="sxs-lookup"><span data-stu-id="b63ae-138">The changes can be verified by listing the assigned roles.</span></span>

```azurecli
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="b63ae-139">Le message indique que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ sur l’étendue ’/subscriptions/{guid}’ » lorsque votre compte ne dispose pas d’autorisations suffisantes pour affecter un rôle. Contactez votre administrateur Azure Active Directory pour gérer les rôles.</span><span class="sxs-lookup"><span data-stu-id="b63ae-139">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="log-in-using-the-service-principal"></a><span data-ttu-id="b63ae-140">Se connecter en tant que principal du service</span><span class="sxs-lookup"><span data-stu-id="b63ae-140">Log in using the service principal</span></span>

<span data-ttu-id="b63ae-141">Vous pouvez tester la connexion et les autorisations du principal du service en ouvrant une session sous ce dernier dans Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b63ae-141">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="b63ae-142">Connectez-vous en tant que nouveau principal du service à l’aide de `appId`, `tenant`et des valeurs des informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="b63ae-142">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="b63ae-143">Les informations d’authentification que vous fournissez changent selon que vous avez choisi de créer le principal du service avec un mot de passe ou un certificat.</span><span class="sxs-lookup"><span data-stu-id="b63ae-143">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="b63ae-144">Pour vous connecter avec un mot de passe, vous devez le fournir en tant que paramètre d’argument.</span><span class="sxs-lookup"><span data-stu-id="b63ae-144">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="b63ae-145">Pour vous connecter avec un certificat, celui-ci doit être disponible localement sous forme de fichier PEM ou DER.</span><span class="sxs-lookup"><span data-stu-id="b63ae-145">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```
## <a name="reset-credentials"></a><span data-ttu-id="b63ae-146">Réinitialiser les informations d’identification</span><span class="sxs-lookup"><span data-stu-id="b63ae-146">Reset credentials</span></span>

<span data-ttu-id="b63ae-147">Si vous oubliez les informations d’identification relatives à un principal de service, il est possible de les réinitialiser à l’aide de la commande [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials).</span><span class="sxs-lookup"><span data-stu-id="b63ae-147">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials) command.</span></span> <span data-ttu-id="b63ae-148">Les mêmes restrictions et options de création d’un principal de service s’appliquent également ici.</span><span class="sxs-lookup"><span data-stu-id="b63ae-148">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
