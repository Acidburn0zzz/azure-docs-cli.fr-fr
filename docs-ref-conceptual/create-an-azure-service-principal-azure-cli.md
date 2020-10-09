---
title: Utilisez des principaux du service Azure avec Azure CLI
description: Découvrez comment créer et utiliser des principaux du service avec l’interface de ligne de commande Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/15/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: f3fb0e589c4a32cc8a8e9e53c0fa3e69bf9576c2
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225947"
---
# <a name="create-an-azure-service-principal-with-the-azure-cli"></a><span data-ttu-id="bc7c4-103">Créer un principal du service Azure à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="bc7c4-103">Create an Azure service principal with the Azure CLI</span></span>

<span data-ttu-id="bc7c4-104">Les outils automatisés qui utilisent les services Azure doivent toujours avoir des autorisations restreintes.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="bc7c4-105">Plutôt que de faire se connecter des applications en tant qu’utilisateur entièrement privilégié, Azure offre des principaux du service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="bc7c4-106">Un principal de service Azure est une identité créée pour une utilisation avec les applications, des services hébergés et des outils automatisés permettant d’accéder aux ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="bc7c4-107">Cet accès est limité par les rôles assignés au principal du service, ce qui vous permet de contrôler quelles ressources sont accessibles et à quel niveau.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="bc7c4-108">Pour des raisons de sécurité, il est toujours recommandé d’utiliser les principaux du service avec des outils automatisés, plutôt que de leur permettre de se connecter avec une identité d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="bc7c4-109">Cet article vous explique les étapes à suivre pour créer, réinitialiser et obtenir des informations sur un principal du service avec l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="bc7c4-110">Créer un principal du service</span><span class="sxs-lookup"><span data-stu-id="bc7c4-110">Create a service principal</span></span>

<span data-ttu-id="bc7c4-111">Créez un principal de service à l’aide de la commande [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="bc7c4-112">Lorsque vous créez un principal de service, vous choisissez le type d’authentification de connexion qu’il utilise.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="bc7c4-113">Si votre compte ne dispose pas d’autorisations pour créer un principal de service, `az ad sp create-for-rbac` vous retournera un message d’erreur contenant « Privilèges insuffisants pour effectuer l’opération ».</span><span class="sxs-lookup"><span data-stu-id="bc7c4-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="bc7c4-114">Contactez votre administrateur Azure Active Directory pour créer un principal de service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="bc7c4-115">Il existe deux types d’authentification disponibles pour les principaux de service : L’authentification basée sur un mot de passe et l’authentification basée sur un certificat.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="bc7c4-116">L’authentification basée sur un mot de passe</span><span class="sxs-lookup"><span data-stu-id="bc7c4-116">Password-based authentication</span></span>

<span data-ttu-id="bc7c4-117">Sans aucun paramètre d’authentification, l’authentification basée sur un mot de passe est utilisée avec un mot de passe aléatoire créé pour vous.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="bc7c4-118">À compter d’Azure CLI 2.0.68, le paramètre `--password` permettant de créer un principal de service avec un mot de passe défini par l’utilisateur __n’est plus pris en charge__ pour empêcher l’utilisation accidentelle de mots de passe faibles.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="bc7c4-119">La sortie d’un principal de service avec l’authentification par mot de passe comprend la clé `password`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="bc7c4-120">__Assurez-vous__ d’avoir copié cette valeur : elle ne pourra être récupérée.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="bc7c4-121">Si vous oubliez le mot de passe, effectuez une [réinitialisation des informations d’identification du principal du service](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="bc7c4-122">Les clés `appId` et `tenant` s’affichent dans la sortie de `az ad sp create-for-rbac` et sont utilisés dans l’authentification du principal du service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="bc7c4-123">Enregistrez leurs valeurs, mais elles peuvent être récupérées à tout moment avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="bc7c4-124">Authentification par certificat</span><span class="sxs-lookup"><span data-stu-id="bc7c4-124">Certificate-based authentication</span></span>

<span data-ttu-id="bc7c4-125">Pour l’authentification basée sur un certificat, utilisez l’argument `--cert`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="bc7c4-126">Cet argument requiert que vous possédiez un certificat existant.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="bc7c4-127">Assurez-vous que n’importe quel outil qui utilise ce principal de service a accès à la clé privée du certificat.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="bc7c4-128">Les certificats doivent être au format ASCII tel que PEM, CER ou DER.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="bc7c4-129">Transmettez le certificat sous forme de chaîne, ou utilisez le format `@path` pour charger le certificat depuis un fichier.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

> [!NOTE]
> <span data-ttu-id="bc7c4-130">Quand un fichier PEM est utilisé, un **CERTIFICAT** doit être ajouté à la **CLÉ PRIVÉE** dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-130">When using a PEM file, the **CERTIFICATE** must be appended to the **PRIVATE KEY** within the file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="bc7c4-131">L’argument `--keyvault` peut être ajouté pour utiliser un certificat dans Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-131">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="bc7c4-132">Dans ce cas, la valeur `--cert` fait référence au nom du certificat.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-132">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="bc7c4-133">Pour créer un certificat _auto-signé_ pour l’authentification, utilisez l’argument `--create-cert` :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-133">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="bc7c4-134">Sortie de la console :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-134">Console output:</span></span>

```
Creating a role assignment under the scope of "/subscriptions/myId"
Please copy C:\myPath\myNewFile.pem to a safe place.
When you run 'az login', provide the file path in the --password argument
{
  "appId": "myAppId",
  "displayName": "myDisplayName",
  "fileWithCertAndPrivateKey": "C:\\myPath\\myNewFile.pem",
  "name": "http://myName",
  "password": null,
  "tenant": "myTenantId"
}
```

<span data-ttu-id="bc7c4-135">Contenu du nouveau fichier PEM :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-135">Contents of the new PEM file:</span></span>
```
-----BEGIN PRIVATE KEY-----
myPrivateKeyValue
-----END PRIVATE KEY-----
-----BEGIN CERTIFICATE-----
myCertificateValue
-----END CERTIFICATE-----
```

> [!NOTE]
> <span data-ttu-id="bc7c4-136">La commande `az ad sp create-for-rbac --create-cert` crée le principal du service et un fichier PEM.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-136">The `az ad sp create-for-rbac --create-cert` command creates the service principal and a PEM file.</span></span> <span data-ttu-id="bc7c4-137">Le fichier PEM contient une **CLÉ PRIVÉE** correctement mise en forme et un **CERTIFICAT**.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-137">The PEM file contains a correctly formatted **PRIVATE KEY** and **CERTIFICATE**.</span></span>

<span data-ttu-id="bc7c4-138">L’argument `--keyvault` peut être ajouté pour stocker le certificat dans Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-138">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="bc7c4-139">Lorsque vous utilisez `--keyvault`, l’argument `--cert` est __requis__.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-139">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="bc7c4-140">À moins que vous ne stockiez le certificat dans Key Vault, la sortie comprend la clé `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-140">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="bc7c4-141">La valeur de cette clé vous indique l’emplacement dans lequel le certificat généré est stocké.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-141">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="bc7c4-142">__Assurez-vous__ d’avoir copié le certificat à un emplacement sécurisé ou vous ne pourrez pas vous connecter avec ce principal de service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-142">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="bc7c4-143">Pour les certificats stockés dans Key Vault, récupérez la clé privée du certificat avec l’[affichage du secret du coffre de clés az](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-143">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="bc7c4-144">Dans Key Vault, le nom du secret du certificat est le même que le nom du certificat.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-144">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="bc7c4-145">Si vous perdez l’accès à la clé privée d’un certificat, effectuez la [réinitialisation des informations d’identification du principal du service](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-145">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="bc7c4-146">Les clés `appId` et `tenant` s’affichent dans la sortie de `az ad sp create-for-rbac` et sont utilisés dans l’authentification du principal du service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-146">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="bc7c4-147">Enregistrez leurs valeurs, mais elles peuvent être récupérées à tout moment avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-147">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="bc7c4-148">Obtenir un principal de service existant</span><span class="sxs-lookup"><span data-stu-id="bc7c4-148">Get an existing service principal</span></span>

<span data-ttu-id="bc7c4-149">Une liste des principaux de service dans un locataire peut être récupérée avec la [liste az ad sp](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-149">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="bc7c4-150">Par défaut, la commande retourne les cents premiers principaux de service de votre locataire.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-150">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="bc7c4-151">Pour obtenir tous les principaux de service d’un locataire, utilisez l’argument `--all`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-151">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="bc7c4-152">Obtenir cette liste peut prendre beaucoup de temps, il est donc recommandé de filtrer la liste avec l’un des arguments suivants :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-152">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="bc7c4-153">`--display-name` demande les principaux de service ayant un _préfixe_ qui correspond au nom fourni.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-153">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="bc7c4-154">Le nom d’affichage d’un principal de service est la valeur définie avec le paramètre `--name` lors de la création.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-154">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="bc7c4-155">Si vous n’avez pas défini `--name` lors de la création du principal de service, le nom du préfixe est `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-155">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="bc7c4-156">`--spn` filtre la correspondance exacte de nom de principal du service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-156">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="bc7c4-157">Le nom de principal du service commence toujours par `https://`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-157">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="bc7c4-158">si la valeur que vous avez utilisé pour `--name` n’était pas un URI, cette valeur est `https://` suivie du nom d’affichage.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-158">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="bc7c4-159">`--show-mine` demande uniquement les principaux du service créés par l’utilisateur connecté.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-159">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="bc7c4-160">`--filter` utilise un filtre OData et effectue un filtrage _côté serveur_.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-160">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="bc7c4-161">Cette méthode est préférable au filtrage côté client avec l’argument `--query` de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-161">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="bc7c4-162">Pour en savoir plus sur les filtres OData, consultez [syntaxe d’expression de filtres OData](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-162">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="bc7c4-163">Les informations retournées pour les objets de principaux du service sont détaillées.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-163">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="bc7c4-164">Pour obtenir uniquement les informations nécessaires pour vous connecter, utilisez la chaîne de requête `[].{id:appId, tenant:appOwnerTenantId}`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-164">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="bc7c4-165">Par exemple, pour obtenir les informations de connexion de tous les principaux du service créés par l’utilisateur actuellement connecté :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-165">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="bc7c4-166">`az ad sp list` ou [affichage az ad sp](/cli/azure/ad/sp#az-ad-sp-show) permettent d’obtenir l’utilisateur et le locataire, mais pas les secrets d’authentification _ou_ la méthode d’authentification.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-166">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="bc7c4-167">Les secrets des certificats dans Key Vault peuvent être récupérés avec [affichage du secret du coffre de clés az](/cli/azure/keyvault/secret#az-keyvault-secret-show), mais aucun autre secret n’est stocké par défaut.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-167">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="bc7c4-168">Si vous oubliez une méthode d’authentification ou un secret, effectuez la [réinitialisation des informations d’identification du principal du service](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-168">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="bc7c4-169">Gérer les rôles du principal du service</span><span class="sxs-lookup"><span data-stu-id="bc7c4-169">Manage service principal roles</span></span>

<span data-ttu-id="bc7c4-170">L’interface de ligne de commande Azure fournit les commandes suivantes de gestion d’attributions de rôle :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-170">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="bc7c4-171">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="bc7c4-171">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="bc7c4-172">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="bc7c4-172">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="bc7c4-173">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="bc7c4-173">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="bc7c4-174">Un principal du service a le rôle **Contributor** (Collaborateur) par défaut.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-174">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="bc7c4-175">Ce rôle dispose des autorisations complètes de lecture et d’écriture dans un compte Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-175">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="bc7c4-176">Le rôle de **Lecteur** est plus restrictif avec un accès en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-176">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="bc7c4-177">Pour plus d’informations sur les rôles et le contrôle d’accès en fonction du rôle, consultez [RBAC : rôles intégrés pour les ressources Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-177">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="bc7c4-178">Cet exemple ajoute le rôle de **Lecteur** et supprime le rôle de **Contributeur** :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-178">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="bc7c4-179">Si votre compte ne dispose pas d’autorisations pour assigner un rôle, un message d’erreur vous indiquera que votre compte « n’est pas autorisé à effectuer l’action ’Microsoft.Authorization/roleAssignments/write’ ». Contactez votre administrateur Azure Active Directory pour gérer les rôles.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-179">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="bc7c4-180">L’ajout d’un rôle ne restreint _pas_ les autorisations précédemment assignées.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-180">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="bc7c4-181">Lors de la restriction des autorisations du principal du service, le rôle de __Contributeur__ dot être supprimé.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-181">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="bc7c4-182">Les modifications peuvent être vérifiées en répertoriant les rôles attribués :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-182">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="bc7c4-183">Se connecter en tant que principal du service</span><span class="sxs-lookup"><span data-stu-id="bc7c4-183">Sign in using a service principal</span></span>

<span data-ttu-id="bc7c4-184">Testez les informations d’identification et les autorisations du nouveau principal du service en vous connectant.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-184">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="bc7c4-185">Pour vous connecter avec un principal de service, vous avez besoin de `appId`, `tenant` ainsi que des informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-185">To sign in with a service principal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="bc7c4-186">Pour vous connecter avec un principal du service utilisant un mot de passe :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-186">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="bc7c4-187">Pour vous connecter avec un certificat, celui-ci doit être disponible localement sous forme de fichier PEM ou DER, ou au format ASCII.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-187">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format.</span></span> <span data-ttu-id="bc7c4-188">Quand un fichier PEM est utilisé, la **CLÉ PRIVÉE** et le **CERTIFICAT** doivent être ajoutés ensemble dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-188">When using a PEM file, the **PRIVATE KEY** and **CERTIFICATE** must be appended together within the file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="bc7c4-189">Pour en savoir plus sur la connexion avec un principal du service, consultez [Se connecter avec l’interface de ligne de commande Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-189">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="create-a-resource-using-service-principal"></a><span data-ttu-id="bc7c4-190">Créer une ressource en utilisant le principal de service</span><span class="sxs-lookup"><span data-stu-id="bc7c4-190">Create a resource using service principal</span></span>

<span data-ttu-id="bc7c4-191">La section suivante fournit un exemple de création d’une ressource pour le [Stockage Azure](/azure/storage/) avec un principal de service, en utilisant les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-191">The following section provides an example of how to create an resource for [Azure Storage](/azure/storage/) with a service principal, using the following commands:</span></span>

* [<span data-ttu-id="bc7c4-192">az login</span><span class="sxs-lookup"><span data-stu-id="bc7c4-192">az login</span></span>](/cli/azure/reference-index?view=azure-cli-latest#az_login)
* [<span data-ttu-id="bc7c4-193">az group create</span><span class="sxs-lookup"><span data-stu-id="bc7c4-193">az group create</span></span>](/cli/azure/group?view=azure-cli-latest#az_group_create)
* [<span data-ttu-id="bc7c4-194">az storage account create</span><span class="sxs-lookup"><span data-stu-id="bc7c4-194">az storage account create</span></span>](/cli/azure/storage/account?view=azure-cli-latest#az_storage_account_create)
* [<span data-ttu-id="bc7c4-195">az storage account keys list</span><span class="sxs-lookup"><span data-stu-id="bc7c4-195">az storage account keys list</span></span>](/cli/azure/storage/account/keys?view=azure-cli-latest#az_storage_account_keys_list)

<span data-ttu-id="bc7c4-196">Pour vous connecter avec un principal de service, vous avez besoin que `appId`, `tenant` et `password` soient retournés comme réponse lorsque vous [avez créé votre principal de service](#sign-in-using-a-service-principal).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-196">To sign in with a service principal, you need the `appId`, `tenant`, and `password` returned as the response when you [created your service principal](#sign-in-using-a-service-principal).</span></span>

1. <span data-ttu-id="bc7c4-197">Connectez-vous en tant que principal du service.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-197">Log in as the service principal.</span></span>

    ```azurecli-interactive
    az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
    ```

1. <span data-ttu-id="bc7c4-198">Créez un groupe de ressources pour y mettre toutes les ressources utilisées pour le même démarrage rapide, le même tutoriel ou le même projet de développement.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-198">Create a resource group to hold all resources used for the same quickstart, tutorial, or development project.</span></span>

    ```azurecli-interactive
    az group create --location WESTUS --name MY_RESOURCE_GROUP
    ```

1. <span data-ttu-id="bc7c4-199">Créez une ressource pour un service Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-199">Create a resource to an Azure service.</span></span> <span data-ttu-id="bc7c4-200">Remplacez `<SERVICENAME>` par le nom du service Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-200">Replace `<SERVICENAME>` with the name of the Azure service.</span></span>

    <span data-ttu-id="bc7c4-201">Pour Stockage Azure, les valeurs valides du paramètre `<KIND>` sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="bc7c4-201">For Azure Storage, valid values for the `<KIND>` parameter are:</span></span>

    * <span data-ttu-id="bc7c4-202">BlobStorage</span><span class="sxs-lookup"><span data-stu-id="bc7c4-202">BlobStorage</span></span>
    * <span data-ttu-id="bc7c4-203">BlockBlobStorage</span><span class="sxs-lookup"><span data-stu-id="bc7c4-203">BlockBlobStorage</span></span>
    * <span data-ttu-id="bc7c4-204">FileStorage</span><span class="sxs-lookup"><span data-stu-id="bc7c4-204">FileStorage</span></span>
    * <span data-ttu-id="bc7c4-205">Stockage</span><span class="sxs-lookup"><span data-stu-id="bc7c4-205">Storage</span></span>
    * <span data-ttu-id="bc7c4-206">StorageV2</span><span class="sxs-lookup"><span data-stu-id="bc7c4-206">StorageV2</span></span>

    ```azurecli-interactive
    az storage account create --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP --kind <KIND> --sku F0 --location WESTUS --yes
    ```

1. <span data-ttu-id="bc7c4-207">Obtenez des clés de ressource pour la nouvelle ressource, que vous utilisez dans votre code pour vous authentifier auprès du service Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-207">Get resource keys for the new resource, which you use in your code to authenticate to the Azure service.</span></span>

    ```azurecli-interactive
    az storage account keys list --name MY_RESOURCE_<SERVICENAME> --resource-group MY_RESOURCE_GROUP
    ```

## <a name="reset-credentials"></a><span data-ttu-id="bc7c4-208">Réinitialiser les informations d’identification</span><span class="sxs-lookup"><span data-stu-id="bc7c4-208">Reset credentials</span></span>

<span data-ttu-id="bc7c4-209">Si vous avez oublié les informations d’identification d’un principal du service, utilisez la [réinitialisation des informations d’identification az ad sp](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="bc7c4-209">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="bc7c4-210">La commande de réinitialisation utilise les mêmes arguments que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="bc7c4-210">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```