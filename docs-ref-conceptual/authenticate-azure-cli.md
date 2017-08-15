---
title: Se connecter avec Azure CLI 2.0
description: Se connecter avec Azure CLI 2.0 sur Linux, Mac ou Windows.
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2017
---
# <a name="log-in-with-azure-cli-20"></a><span data-ttu-id="01c50-104">Se connecter avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="01c50-104">Log in with Azure CLI 2.0</span></span>

<span data-ttu-id="01c50-105">Il existe plusieurs manières de se connecter et de s’authentifier auprès d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="01c50-105">There are several ways to log in and authenticate with the Azure CLI.</span></span> <span data-ttu-id="01c50-106">Le plus simple est de vous connecter de manière interactive par l’intermédiaire de votre navigateur, ou de vous connecter à la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="01c50-106">The simplest way to get started is to log in interactively through your browser, or to log in at the command line.</span></span> <span data-ttu-id="01c50-107">Nous vous recommandons d’utiliser des principaux du service, qui offrent un moyen de créer des comptes non interactifs que vous pouvez utiliser pour manipuler les ressources.</span><span class="sxs-lookup"><span data-stu-id="01c50-107">Our recommended approach is to use service principals, which provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="01c50-108">En accordant uniquement les autorisations nécessaires à un principal du service, vous pouvez garantir que vos scripts d’automatisation sont encore plus sûrs.</span><span class="sxs-lookup"><span data-stu-id="01c50-108">By granting just the appropriate permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="01c50-109">Les commandes que vous exécutez avec l’interface de ligne de commande sont exécutées sur votre abonnement par défaut.</span><span class="sxs-lookup"><span data-stu-id="01c50-109">Commands that you run with the CLI are run against your default subscription.</span></span>  <span data-ttu-id="01c50-110">Si vous avez plusieurs abonnements, vous souhaiterez peut-être [confirmer votre abonnement par défaut](manage-azure-subscriptions-azure-cli.md) et le changer en conséquence.</span><span class="sxs-lookup"><span data-stu-id="01c50-110">If you have more than one subscription, you may want to [confirm your default subscription](manage-azure-subscriptions-azure-cli.md) and change it appropriately.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="01c50-111">Connexion interactive</span><span class="sxs-lookup"><span data-stu-id="01c50-111">Interactive log-in</span></span>

<span data-ttu-id="01c50-112">Connectez-vous de manière interactive à partir de votre navigateur web.</span><span class="sxs-lookup"><span data-stu-id="01c50-112">Log in interactively from your web browser.</span></span>

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a><span data-ttu-id="01c50-113">Ligne de commande</span><span class="sxs-lookup"><span data-stu-id="01c50-113">Command line</span></span>

<span data-ttu-id="01c50-114">Fournissez vos informations d’identification sur la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="01c50-114">Provide your credentials on the command line.</span></span>

> [!Note]
> <span data-ttu-id="01c50-115">Cette approche ne fonctionne pas avec les comptes Microsoft ou les comptes pour lesquels l’authentification à deux facteurs est activée.</span><span class="sxs-lookup"><span data-stu-id="01c50-115">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a><span data-ttu-id="01c50-116">Connexion avec un principal du service</span><span class="sxs-lookup"><span data-stu-id="01c50-116">Logging in with a service principal</span></span>

<span data-ttu-id="01c50-117">Les principaux du service sont comme des comptes d’utilisateur auxquels vous pouvez appliquer des règles à l’aide d’Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="01c50-117">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span>
<span data-ttu-id="01c50-118">L’authentification avec un principal du service est le meilleur moyen de sécuriser l’utilisation de vos ressources Azure à partir de vos applications ou scripts qui manipulent des ressources.</span><span class="sxs-lookup"><span data-stu-id="01c50-118">Authenticating with a service principal is the best way to secure the usage of your Azure resources from either your scripts or applications that manipulate resources.</span></span>
<span data-ttu-id="01c50-119">Vous définissez les rôles dont vous souhaitez que vos utilisateurs disposent par l’intermédiaire de l’ensemble de commandes `az role`.</span><span class="sxs-lookup"><span data-stu-id="01c50-119">You define the roles you want your users to have via the `az role` set of commands.</span></span>
<span data-ttu-id="01c50-120">Pour en savoir plus et pour obtenir des exemples de rôles de principal du service, consultez nos [articles de référence de rôle az](https://docs.microsoft.com/cli/azure/role.md).</span><span class="sxs-lookup"><span data-stu-id="01c50-120">You can learn more and see examples of service principal roles in our [az role reference articles](https://docs.microsoft.com/cli/azure/role.md).</span></span>

1. <span data-ttu-id="01c50-121">Si vous n’avez pas encore de principal du service, [créez-en un](create-an-azure-service-principal-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="01c50-121">If you don't already have a service principal, [create one](create-an-azure-service-principal-azure-cli.md).</span></span>

1. <span data-ttu-id="01c50-122">Connectez-vous avec un principal du service.</span><span class="sxs-lookup"><span data-stu-id="01c50-122">Log in with the service principal.</span></span>

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   <span data-ttu-id="01c50-123">Pour obtenir votre locataire, connectez-vous de manière interactive, puis obtenez l’ID de locataire de votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="01c50-123">To get your tenant, log in interactively and then get the tenantId from your subscription.</span></span>

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```