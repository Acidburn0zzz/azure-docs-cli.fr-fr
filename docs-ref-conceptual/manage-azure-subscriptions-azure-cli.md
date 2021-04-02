---
title: Gérer des abonnements Azure avec Azure CLI
description: Découvrez les locataires, les utilisateurs et les abonnements Azure. Utilisez Azure CLI pour gérer vos abonnements, créer des groupes d’administration et verrouiller des abonnements.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: a2a4467bc25fb8da8ced0c7b8cb6c4db9eb35e64
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581833"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a><span data-ttu-id="b8985-104">Utiliser des abonnements Azure avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b8985-104">Use Azure subscriptions with Azure CLI</span></span>

<span data-ttu-id="b8985-105">Vous avez peut-être plusieurs abonnements dans Azure.</span><span class="sxs-lookup"><span data-stu-id="b8985-105">You might have multiple subscriptions within Azure.</span></span> <span data-ttu-id="b8985-106">Soit vous faites partie de plusieurs organisations, soit votre organisation divise l’accès à certaines ressources selon des groupes.</span><span class="sxs-lookup"><span data-stu-id="b8985-106">You can be part of more than one organization or your organization might divide access to certain resources across groupings.</span></span> <span data-ttu-id="b8985-107">Azure CLI prend en charge la sélection d’un abonnement à la fois au niveau global et par commande.</span><span class="sxs-lookup"><span data-stu-id="b8985-107">The Azure CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="b8985-108">Pour plus d’informations sur les abonnements, la facturation et la gestion des coûts, consultez la [documentation sur la facturation et la gestion des coûts](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="b8985-108">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="b8985-109">Locataires, utilisateurs et abonnements</span><span class="sxs-lookup"><span data-stu-id="b8985-109">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="b8985-110">Un _locataire_ correspond à l’entité d’Azure Active Directory qui inclut une organisation complète.</span><span class="sxs-lookup"><span data-stu-id="b8985-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="b8985-111">Un locataire a un ou plusieurs _abonnements_ et _utilisateurs_.</span><span class="sxs-lookup"><span data-stu-id="b8985-111">A tenant has one or more _subscription_ and _user_.</span></span> <span data-ttu-id="b8985-112">Un utilisateur est un individu qui n’est associé qu’à un seul locataire, c’est-à-dire à l’organisation auquel il appartient.</span><span class="sxs-lookup"><span data-stu-id="b8985-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="b8985-113">Les utilisateurs correspondent aux comptes qui se connectent à Azure afin de configurer, de gérer et d’utiliser des ressources.</span><span class="sxs-lookup"><span data-stu-id="b8985-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span> <span data-ttu-id="b8985-114">Un utilisateur peut avoir accès à plusieurs _abonnements_, qui sont les contrats avec Microsoft pour utiliser les services de cloud, y compris Azure.</span><span class="sxs-lookup"><span data-stu-id="b8985-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="b8985-115">Chaque ressource est associée à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8985-115">Every resource is associated with a subscription.</span></span>

* <span data-ttu-id="b8985-116">Pour en savoir plus sur les différences entre les locataires, les utilisateurs et les abonnements, consultez le [Dictionnaire de terminologie cloud Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="b8985-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
* <span data-ttu-id="b8985-117">Pour savoir comment ajouter un nouvel abonnement à votre locataire Azure Active Directory, consultez [Associer ou ajouter un abonnement Azure à votre locataire Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b8985-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
* <span data-ttu-id="b8985-118">Pour savoir comment se connecter à un locataire en particulier, consultez [Se connecter avec Azure CLI](./authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b8985-118">To learn how to sign in to a specific tenant, see [Sign in with the Azure CLI](./authenticate-azure-cli.md).</span></span>

## <a name="commands-in-a-subscription"></a><span data-ttu-id="b8985-119">Commandes dans un abonnement</span><span class="sxs-lookup"><span data-stu-id="b8985-119">Commands in a subscription</span></span>

<span data-ttu-id="b8985-120">De nombreuses commandes Azure CLI agissent au sein d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8985-120">Many Azure CLI commands act within a subscription.</span></span> <span data-ttu-id="b8985-121">Vous pouvez toujours spécifier dans quel abonnement agir à l’aide du paramètre **subscription** dans votre commande.</span><span class="sxs-lookup"><span data-stu-id="b8985-121">You can always specify which subscription to work in by using the **subscription** parameter in your command.</span></span> <span data-ttu-id="b8985-122">Ce paramètre est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b8985-122">That parameter is optional.</span></span> <span data-ttu-id="b8985-123">Si vous ne spécifiez pas d’abonnement, la commande utilise votre abonnement actuel et actif.</span><span class="sxs-lookup"><span data-stu-id="b8985-123">If you don't specify a subscription, the command uses your current, active subscription.</span></span>

<span data-ttu-id="b8985-124">Pour voir l’abonnement que vous êtes en train d’utiliser, exécutez la commande [az account show](/cli/azure/account#az_account_show) :</span><span class="sxs-lookup"><span data-stu-id="b8985-124">To see the subscription you're currently using, run the [az account show](/cli/azure/account#az_account_show) command:</span></span>

```azurecli
az account show --output table
```

> [!TIP]
> <span data-ttu-id="b8985-125">Le paramètre `--output` est un paramètre global, disponible pour toutes les commandes.</span><span class="sxs-lookup"><span data-stu-id="b8985-125">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="b8985-126">La valeur **table** présente la sortie dans un format convivial.</span><span class="sxs-lookup"><span data-stu-id="b8985-126">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="b8985-127">Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="b8985-127">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="b8985-128">Les abonnements contiennent des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="b8985-128">Subscriptions contain resource groups.</span></span> <span data-ttu-id="b8985-129">Un groupe de ressources Azure est un conteneur réunissant les ressources associées d’une solution Azure.</span><span class="sxs-lookup"><span data-stu-id="b8985-129">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="b8985-130">Si votre commande utilisent des ressources contenues dans votre abonnement actif, vous n’avez pas besoin de spécifier `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="b8985-130">If your command works with resources in your active subscription, you don't need to specify `--subscription`.</span></span>

<span data-ttu-id="b8985-131">Cette commande crée un compte de stockage dans le groupe de ressources spécifié :</span><span class="sxs-lookup"><span data-stu-id="b8985-131">This command creates a storage account in the specified resource group:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

<span data-ttu-id="b8985-132">Si le groupe de stockage ne fait pas partie de votre abonnement actif actuel, cette commande échoue.</span><span class="sxs-lookup"><span data-stu-id="b8985-132">If the storage group isn't part of your current active subscription, this command fails.</span></span>

<span data-ttu-id="b8985-133">Si nécessaire, modifiez l’abonnement actif, comme décrit dans la section suivante, ou bien spécifiez l’abonnement dans la commande :</span><span class="sxs-lookup"><span data-stu-id="b8985-133">If necessary, change the active subscription, as described in the next section, or specify the subscription in the command:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a><span data-ttu-id="b8985-134">Modifier l’abonnement actif</span><span class="sxs-lookup"><span data-stu-id="b8985-134">Change the active subscription</span></span>

<span data-ttu-id="b8985-135">Vous pouvez modifier votre abonnement actif à l’aide de la commande [az account set](/cli/azure/account#az_account_set).</span><span class="sxs-lookup"><span data-stu-id="b8985-135">You can change your active subscription by using the [az account set](/cli/azure/account#az_account_set) command.</span></span>

<span data-ttu-id="b8985-136">Obtenez une liste de vos abonnements à l’aide de la commande [az account list](/cli/azure/account#az_account_list) :</span><span class="sxs-lookup"><span data-stu-id="b8985-136">Get a list of your subscriptions with the [az account list](/cli/azure/account#az_account_list) command:</span></span>

```azurecli
az account list --output table
```

<span data-ttu-id="b8985-137">Cette commande liste tous les abonnements auxquels vous pouvez accéder.</span><span class="sxs-lookup"><span data-stu-id="b8985-137">This command lists all the subscriptions you can access.</span></span> <span data-ttu-id="b8985-138">Votre abonnement actif est marqué comme `True` dans la colonne `IsDefault`.</span><span class="sxs-lookup"><span data-stu-id="b8985-138">Your active subscription is marked as `True` in the `IsDefault` column.</span></span> <span data-ttu-id="b8985-139">Si, contre toute attente, il manque un abonnement, ajoutez le paramètre `--refresh` pour obtenir la liste la plus récente des abonnements.</span><span class="sxs-lookup"><span data-stu-id="b8985-139">If you don't see a subscription you expect, add the `--refresh` parameter to get the most current list of subscriptions.</span></span>

<span data-ttu-id="b8985-140">Pour basculer vers un autre abonnement, utilisez [az account set](/cli/azure/account#az_account_set) avec l’ID ou le nom de l’abonnement vers lequel vous voulez basculer.</span><span class="sxs-lookup"><span data-stu-id="b8985-140">To switch to a different subscription, use [az account set](/cli/azure/account#az_account_set) with the subscription ID or name you want to switch to.</span></span>

```azurecli
az account set --subscription "My Demos"
```

<span data-ttu-id="b8985-141">Vos abonnements ont à la fois un nom et un ID, qui est un GUID.</span><span class="sxs-lookup"><span data-stu-id="b8985-141">Your subscriptions have both a name and an ID, which is a GUID.</span></span> <span data-ttu-id="b8985-142">Vous pouvez utiliser l’un ou l’autre pour ces commandes.</span><span class="sxs-lookup"><span data-stu-id="b8985-142">You can use either for these commands.</span></span> <span data-ttu-id="b8985-143">Si vous utilisez un nom qui comprend des espaces, utilisez des guillemets.</span><span class="sxs-lookup"><span data-stu-id="b8985-143">If you use a name that includes spaces, use quotation marks.</span></span>

<span data-ttu-id="b8985-144">Si vous réexécutez la commande [az account list](/cli/azure/account#az_account_list), la colonne `IsDefault` indique votre abonnement actif actuel.</span><span class="sxs-lookup"><span data-stu-id="b8985-144">If you run the [az account list](/cli/azure/account#az_account_list) command again, the `IsDefault` column shows your current active subscription.</span></span>

## <a name="create-management-groups"></a><span data-ttu-id="b8985-145">Créer des groupes d’administration</span><span class="sxs-lookup"><span data-stu-id="b8985-145">Create management groups</span></span>

<span data-ttu-id="b8985-146">Les groupes d’administration Azure contiennent des abonnements.</span><span class="sxs-lookup"><span data-stu-id="b8985-146">Azure management groups contain subscriptions.</span></span> <span data-ttu-id="b8985-147">Les groupes d’administration offrent un moyen de gérer l’accès, les stratégies et la conformité de ces abonnements.</span><span class="sxs-lookup"><span data-stu-id="b8985-147">Management groups provide a way to manage access, policies, and compliance for those subscriptions.</span></span> <span data-ttu-id="b8985-148">Pour plus d’informations, consultez [Présentation des groupes d’administration Azure](/azure/governance/management-groups/overview).</span><span class="sxs-lookup"><span data-stu-id="b8985-148">For more information, see [What are Azure management groups](/azure/governance/management-groups/overview).</span></span>

<span data-ttu-id="b8985-149">Utilisez les commandes [az account management-group](/cli/azure/account/management-group) pour créer et gérer des groupes d’administration Azure.</span><span class="sxs-lookup"><span data-stu-id="b8985-149">Use the [az account management-group](/cli/azure/account/management-group) commands to create and manage Azure Management Groups.</span></span>

<span data-ttu-id="b8985-150">Vous pouvez créer un groupe d’administration pour plusieurs de vos abonnements à l’aide de la commande [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) :</span><span class="sxs-lookup"><span data-stu-id="b8985-150">You can create a management group for several of your subscriptions by using the [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) command:</span></span>

```azurecli
az account management-group create --name Contoso01
```

<span data-ttu-id="b8985-151">Pour afficher tous vos groupes d’administration, utilisez la commande [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) :</span><span class="sxs-lookup"><span data-stu-id="b8985-151">To see all your management groups, use the [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) command:</span></span>

```azurecli
az account management-group list
```

<span data-ttu-id="b8985-152">Ajoutez des abonnements à votre nouveau groupe en utilisant la commande [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) :</span><span class="sxs-lookup"><span data-stu-id="b8985-152">Add subscriptions to your new group by using the [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) command:</span></span>

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

<span data-ttu-id="b8985-153">Pour supprimer un abonnement, utilisez la commande [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) :</span><span class="sxs-lookup"><span data-stu-id="b8985-153">To remove a subscription, use the [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) command:</span></span>

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

<span data-ttu-id="b8985-154">Pour supprimer un groupe d’administration, exécutez la commande [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) :</span><span class="sxs-lookup"><span data-stu-id="b8985-154">To remove a management group, run the [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) command:</span></span>

```azurecli
az account management-group delete --name Contoso01
```

<span data-ttu-id="b8985-155">La suppression d’un abonnement ou d’un groupe d’administration n’entraîne pas la suppression définitive ni la désactivation de cet abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8985-155">Removing a subscription or deleting a management group doesn't delete or deactivate a subscription.</span></span>

## <a name="set-a-subscription-lock"></a><span data-ttu-id="b8985-156">Définir un verrou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="b8985-156">Set a subscription lock</span></span>

<span data-ttu-id="b8985-157">En tant qu’administrateur, vous pouvez avoir besoin de verrouiller un abonnement pour empêcher des utilisateurs de le supprimer ou de le modifier.</span><span class="sxs-lookup"><span data-stu-id="b8985-157">As an administrator, you may need to lock a subscription to prevent users from deleting or modifying it.</span></span> <span data-ttu-id="b8985-158">Pour plus d’informations, consultez [Verrouiller les ressources pour empêcher les modifications inattendues](/azure/azure-resource-manager/management/lock-resources).</span><span class="sxs-lookup"><span data-stu-id="b8985-158">For more information, see [Lock resources to prevent unexpected changes](/azure/azure-resource-manager/management/lock-resources).</span></span>

<span data-ttu-id="b8985-159">Dans Azure CLI, utilisez les commandes [az account lock](/cli/azure/account/lock).</span><span class="sxs-lookup"><span data-stu-id="b8985-159">In Azure CLI, use the [az account lock](/cli/azure/account/lock) commands.</span></span> <span data-ttu-id="b8985-160">Par exemple, la commande [az account lock create](/cli/azure/account/lock#az_account_lock_create) peut empêcher les utilisateurs de supprimer un abonnement :</span><span class="sxs-lookup"><span data-stu-id="b8985-160">For instance, the [az account lock create](/cli/azure/account/lock#az_account_lock_create) command can prevent users from deleting a subscription:</span></span>

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> <span data-ttu-id="b8985-161">Vous avez besoin des autorisations appropriées pour créer ou modifier des verrous.</span><span class="sxs-lookup"><span data-stu-id="b8985-161">You need to have appropriate permissions to create or change locks.</span></span>

<span data-ttu-id="b8985-162">Pour afficher les verrous actuellement définis sur votre abonnement, utilisez la commande [az account lock list](/cli/azure/account/lock#az_account_lock_list) :</span><span class="sxs-lookup"><span data-stu-id="b8985-162">To see the current locks on your subscription, use the [az account lock list](/cli/azure/account/lock#az_account_lock_list) command:</span></span>

```azurecli
az account lock list --output table
```

<span data-ttu-id="b8985-163">Si vous définissez un compte en tant que compte en lecture seule, cela revient à attribuer les autorisations du rôle Lecteur à tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="b8985-163">If you make an account read-only, the result resembles assigning permissions of the Reader role to all users.</span></span> <span data-ttu-id="b8985-164">Pour en savoir plus sur la définition d’autorisations pour des utilisateurs individuels et des rôles, consultez [Ajouter ou supprimer des attributions de rôle Azure à l’aide d’Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span><span class="sxs-lookup"><span data-stu-id="b8985-164">To learn about setting permissions for individual users and roles, see [Add or remove Azure role assignments using Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span></span>

<span data-ttu-id="b8985-165">Pour afficher les détails d’un verrou, utilisez la commande [az account lock show](/cli/azure/account/lock#az_account_lock_show) :</span><span class="sxs-lookup"><span data-stu-id="b8985-165">To see details for a lock, use the [az account lock show](/cli/azure/account/lock#az_account_lock_show) command:</span></span>

```azurecli
az account lock show --name "Cannot delete subscription"
```

<span data-ttu-id="b8985-166">Vous pouvez supprimer un verrou à l’aide de la commande [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) :</span><span class="sxs-lookup"><span data-stu-id="b8985-166">You can remove a lock by using the [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) command:</span></span>

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a><span data-ttu-id="b8985-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b8985-167">See also</span></span>

* [<span data-ttu-id="b8985-168">Dictionnaire de la terminologie cloud Azure</span><span class="sxs-lookup"><span data-stu-id="b8985-168">Azure cloud terminology dictionary</span></span>](/azure/azure-glossary-cloud-terminology)
* [<span data-ttu-id="b8985-169">Associer ou ajouter un abonnement Azure à votre locataire Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b8985-169">Associate or add an Azure subscription to your Azure Active Directory tenant</span></span>](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [<span data-ttu-id="b8985-170">Se connecter avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b8985-170">Sign in with Azure CLI</span></span>](./authenticate-azure-cli.md)
