---
title: Notes de publication d’Azure CLI 2.0
description: En savoir plus sur les dernières mises à jour d’Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d0f8c01495cc95ecfbf6a41d510eb4bc54d47ba2
ms.sourcegitcommit: 8019690502e9f89c083839d83a0a245cc812e8b6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/01/2018
ms.locfileid: "39392351"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="e2c84-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e2c84-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e2c84-104">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-104">July 31, 2018</span></span>

<span data-ttu-id="e2c84-105">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e2c84-105">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-106">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-106">ACR</span></span>

* <span data-ttu-id="e2c84-107">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-107">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e2c84-108">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="e2c84-108">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-109">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-109">ACS</span></span>

* <span data-ttu-id="e2c84-110">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="e2c84-110">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-111">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-111">Batch</span></span>

* <span data-ttu-id="e2c84-112">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e2c84-112">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-113">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-113">Container</span></span>

* <span data-ttu-id="e2c84-114">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="e2c84-114">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-115">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-115">Network</span></span>

* <span data-ttu-id="e2c84-116">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e2c84-116">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e2c84-117">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-117">Resource</span></span>

* <span data-ttu-id="e2c84-118">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="e2c84-118">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e2c84-119">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="e2c84-119">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-120">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-120">Role</span></span>

* <span data-ttu-id="e2c84-121">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-121">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e2c84-122">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="e2c84-122">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e2c84-123">Recherche</span><span class="sxs-lookup"><span data-stu-id="e2c84-123">Search</span></span>

* <span data-ttu-id="e2c84-124">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="e2c84-124">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e2c84-125">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e2c84-125">Service Bus</span></span>

* <span data-ttu-id="e2c84-126">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="e2c84-126">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e2c84-127">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-127">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e2c84-128">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="e2c84-128">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e2c84-129">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-129">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-130">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-130">Storage</span></span>

* <span data-ttu-id="e2c84-131">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="e2c84-131">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e2c84-132">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e2c84-132">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-133">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-133">VM</span></span>

* <span data-ttu-id="e2c84-134">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-134">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e2c84-135">Ajout d’une prise en charge à `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="e2c84-135">Added support for support `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e2c84-136">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="e2c84-136">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e2c84-137">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-137">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e2c84-138">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-138">July 18, 2018</span></span>

<span data-ttu-id="e2c84-139">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e2c84-139">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-140">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-140">Core</span></span>

* <span data-ttu-id="e2c84-141">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="e2c84-141">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e2c84-142">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="e2c84-142">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e2c84-143">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="e2c84-143">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-144">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-144">ACR</span></span>

* <span data-ttu-id="e2c84-145">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="e2c84-145">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e2c84-146">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="e2c84-146">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e2c84-147">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="e2c84-147">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e2c84-148">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="e2c84-148">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-149">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-149">ACS</span></span>

* <span data-ttu-id="e2c84-150">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="e2c84-150">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-151">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-151">AppService</span></span>

* <span data-ttu-id="e2c84-152">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="e2c84-152">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-153">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-153">Batch</span></span>

* <span data-ttu-id="e2c84-154">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e2c84-154">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e2c84-155">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="e2c84-155">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e2c84-156">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-156">Batch AI</span></span>

* <span data-ttu-id="e2c84-157">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="e2c84-157">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-158">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-158">Container</span></span>

* <span data-ttu-id="e2c84-159">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="e2c84-159">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e2c84-160">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="e2c84-160">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-161">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-161">Network</span></span>

* <span data-ttu-id="e2c84-162">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-162">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e2c84-163">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="e2c84-163">Added `network nic wait`</span></span>
* <span data-ttu-id="e2c84-164">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-164">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e2c84-165">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-165">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e2c84-166">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-166">Resource</span></span>

* <span data-ttu-id="e2c84-167">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e2c84-167">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e2c84-168">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e2c84-168">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e2c84-169">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="e2c84-169">Added `deployment wait` command</span></span>
* <span data-ttu-id="e2c84-170">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e2c84-170">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-171">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-171">SQL</span></span>

* <span data-ttu-id="e2c84-172">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-172">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e2c84-173">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="e2c84-173">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e2c84-174">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="e2c84-174">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-175">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-175">Storage</span></span>

* <span data-ttu-id="e2c84-176">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="e2c84-176">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-177">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-177">VM</span></span>

* <span data-ttu-id="e2c84-178">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-178">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e2c84-179">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-179">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e2c84-180">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="e2c84-180">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e2c84-181">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-181">July 3, 2018</span></span>

<span data-ttu-id="e2c84-182">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e2c84-182">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e2c84-183">AKS</span><span class="sxs-lookup"><span data-stu-id="e2c84-183">AKS</span></span>

* <span data-ttu-id="e2c84-184">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-184">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e2c84-185">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-185">July 3, 2018</span></span>

<span data-ttu-id="e2c84-186">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e2c84-186">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-187">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-187">Core</span></span>

* <span data-ttu-id="e2c84-188">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-188">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-189">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-189">ACR</span></span>

* <span data-ttu-id="e2c84-190">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="e2c84-190">Added polling build status</span></span>
* <span data-ttu-id="e2c84-191">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="e2c84-191">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e2c84-192">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e2c84-192">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-193">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-193">ACS</span></span>

* <span data-ttu-id="e2c84-194">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-194">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e2c84-195">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-195">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e2c84-196">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-196">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e2c84-197">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="e2c84-197">Added `--listen-port` support</span></span>
* <span data-ttu-id="e2c84-198">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-198">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e2c84-199">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="e2c84-199">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e2c84-200">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="e2c84-200">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-201">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-201">AppService</span></span>

* <span data-ttu-id="e2c84-202">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="e2c84-202">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e2c84-203">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="e2c84-203">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e2c84-204">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e2c84-204">Backup</span></span>

* <span data-ttu-id="e2c84-205">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="e2c84-205">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e2c84-206">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-206">BatchAI</span></span>

* <span data-ttu-id="e2c84-207">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-207">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e2c84-208">Cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-208">Cloud</span></span>

* <span data-ttu-id="e2c84-209">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-209">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-210">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-210">Container</span></span>

* <span data-ttu-id="e2c84-211">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="e2c84-211">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e2c84-212">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="e2c84-212">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e2c84-213">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="e2c84-213">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-214">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-214">Extension</span></span>

* <span data-ttu-id="e2c84-215">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="e2c84-215">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-216">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-216">Network</span></span>

* <span data-ttu-id="e2c84-217">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e2c84-217">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e2c84-218">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e2c84-218">Rdbms</span></span>

* <span data-ttu-id="e2c84-219">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e2c84-219">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-220">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-220">Resource</span></span>

* <span data-ttu-id="e2c84-221">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="e2c84-221">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-222">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-222">VM</span></span>

* <span data-ttu-id="e2c84-223">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="e2c84-223">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e2c84-224">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-224">June 25, 2018</span></span>

<span data-ttu-id="e2c84-225">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e2c84-225">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e2c84-226">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-226">CLI</span></span>

* <span data-ttu-id="e2c84-227">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-227">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e2c84-228">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-228">June 19, 2018</span></span>

<span data-ttu-id="e2c84-229">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e2c84-229">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-230">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-230">Core</span></span>

* <span data-ttu-id="e2c84-231">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-231">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-232">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-232">ACR</span></span>

* <span data-ttu-id="e2c84-233">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="e2c84-233">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e2c84-234">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-234">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-235">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-235">ACS</span></span>

* <span data-ttu-id="e2c84-236">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-236">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e2c84-237">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-237">Added `--update` support</span></span>
* <span data-ttu-id="e2c84-238">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="e2c84-238">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e2c84-239">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="e2c84-239">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e2c84-240">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="e2c84-240">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e2c84-241">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e2c84-241">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e2c84-242">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e2c84-242">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e2c84-243">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e2c84-243">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-244">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-244">AppService</span></span>

* <span data-ttu-id="e2c84-245">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="e2c84-245">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e2c84-246">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="e2c84-246">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-247">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-247">Batch</span></span>

* <span data-ttu-id="e2c84-248">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-248">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e2c84-249">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-249">Batch AI</span></span>

* <span data-ttu-id="e2c84-250">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="e2c84-250">Added support for workspaces.</span></span> <span data-ttu-id="e2c84-251">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="e2c84-251">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e2c84-252">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="e2c84-252">Added support for experiments.</span></span> <span data-ttu-id="e2c84-253">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="e2c84-253">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e2c84-254">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="e2c84-254">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e2c84-255">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-255">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e2c84-256">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="e2c84-256">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e2c84-257">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="e2c84-257">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e2c84-258">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-258">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e2c84-259">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="e2c84-259">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e2c84-260">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-260">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e2c84-261">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="e2c84-261">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e2c84-262">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-262">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e2c84-263">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="e2c84-263">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e2c84-264">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="e2c84-264">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e2c84-265">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="e2c84-265">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e2c84-266">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-266">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e2c84-267">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="e2c84-267">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="e2c84-268">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="e2c84-268">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="e2c84-269">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e2c84-269">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e2c84-270">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e2c84-270">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e2c84-271">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="e2c84-271">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e2c84-272">Cartes</span><span class="sxs-lookup"><span data-stu-id="e2c84-272">Maps</span></span>

* <span data-ttu-id="e2c84-273">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="e2c84-273">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-274">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-274">Network</span></span>

* <span data-ttu-id="e2c84-275">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="e2c84-275">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e2c84-276">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="e2c84-276">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e2c84-277">#6502</span><span class="sxs-lookup"><span data-stu-id="e2c84-277">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e2c84-278">Réservations</span><span class="sxs-lookup"><span data-stu-id="e2c84-278">Reservations</span></span>

* <span data-ttu-id="e2c84-279">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-279">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e2c84-280">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-280">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e2c84-281">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="e2c84-281">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e2c84-282">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e2c84-282">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e2c84-283">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e2c84-283">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e2c84-284">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-284">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-285">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-285">Role</span></span>

* <span data-ttu-id="e2c84-286">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-286">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-287">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-287">SQL</span></span>

* <span data-ttu-id="e2c84-288">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-288">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-289">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-289">Storage</span></span>

* <span data-ttu-id="e2c84-290">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="e2c84-290">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-291">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-291">VM</span></span>

* <span data-ttu-id="e2c84-292">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-292">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e2c84-293">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="e2c84-293">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e2c84-294">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="e2c84-294">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e2c84-295">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-295">June 13, 2018</span></span>

<span data-ttu-id="e2c84-296">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e2c84-296">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-297">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-297">Core</span></span>

* <span data-ttu-id="e2c84-298">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-298">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e2c84-299">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-299">June 13, 2018</span></span>

<span data-ttu-id="e2c84-300">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e2c84-300">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e2c84-301">AKS</span><span class="sxs-lookup"><span data-stu-id="e2c84-301">AKS</span></span>

* <span data-ttu-id="e2c84-302">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-302">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e2c84-303">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="e2c84-303">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e2c84-304">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-304">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e2c84-305">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-305">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e2c84-306">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-306">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-307">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-307">AppService</span></span>

* <span data-ttu-id="e2c84-308">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="e2c84-308">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e2c84-309">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-309">June 5, 2018</span></span>

<span data-ttu-id="e2c84-310">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e2c84-310">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-311">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-311">Interactive</span></span>

* <span data-ttu-id="e2c84-312">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="e2c84-312">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e2c84-313">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-313">June 5, 2018</span></span>

<span data-ttu-id="e2c84-314">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e2c84-314">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-315">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-315">Core</span></span>

* <span data-ttu-id="e2c84-316">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="e2c84-316">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e2c84-317">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="e2c84-317">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-318">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-318">ACR</span></span>

* <span data-ttu-id="e2c84-319">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="e2c84-319">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e2c84-320">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="e2c84-320">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e2c84-321">AKS</span><span class="sxs-lookup"><span data-stu-id="e2c84-321">AKS</span></span>

* <span data-ttu-id="e2c84-322">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="e2c84-322">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-323">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-323">Batch</span></span>

* <span data-ttu-id="e2c84-324">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e2c84-324">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-325">IOT</span><span class="sxs-lookup"><span data-stu-id="e2c84-325">IOT</span></span>

* <span data-ttu-id="e2c84-326">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="e2c84-326">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-327">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-327">Network</span></span>

* <span data-ttu-id="e2c84-328">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="e2c84-328">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e2c84-329">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e2c84-329">Policy Insights</span></span>

* <span data-ttu-id="e2c84-330">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-330">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e2c84-331">ARM</span><span class="sxs-lookup"><span data-stu-id="e2c84-331">ARM</span></span>

* <span data-ttu-id="e2c84-332">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-332">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-333">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-333">SQL</span></span>

* <span data-ttu-id="e2c84-334">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="e2c84-334">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e2c84-335">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="e2c84-335">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e2c84-336">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-336">Storage</span></span>

* <span data-ttu-id="e2c84-337">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="e2c84-337">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-338">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-338">VM</span></span>

* <span data-ttu-id="e2c84-339">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="e2c84-339">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e2c84-340">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-340">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e2c84-341">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-341">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e2c84-342">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-342">May 22, 2018</span></span>

<span data-ttu-id="e2c84-343">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e2c84-343">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-344">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-344">Core</span></span>

* <span data-ttu-id="e2c84-345">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="e2c84-345">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-346">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-346">ACS</span></span>

* <span data-ttu-id="e2c84-347">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="e2c84-347">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e2c84-348">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="e2c84-348">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-349">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-349">AppService</span></span>

* <span data-ttu-id="e2c84-350">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="e2c84-350">Improved generic update commands</span></span>
* <span data-ttu-id="e2c84-351">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="e2c84-351">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-352">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-352">Container</span></span>

* <span data-ttu-id="e2c84-353">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="e2c84-353">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e2c84-354">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-354">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-355">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-355">Extension</span></span>

* <span data-ttu-id="e2c84-356">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="e2c84-356">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-357">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-357">Interactive</span></span>

* <span data-ttu-id="e2c84-358">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="e2c84-358">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e2c84-359">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="e2c84-359">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-360">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-360">KeyVault</span></span>

* <span data-ttu-id="e2c84-361">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="e2c84-361">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-362">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-362">Network</span></span>

* <span data-ttu-id="e2c84-363">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e2c84-363">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e2c84-364">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e2c84-364">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-365">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-365">SQL</span></span>

* <span data-ttu-id="e2c84-366">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="e2c84-366">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e2c84-367">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e2c84-367">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e2c84-368">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="e2c84-368">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e2c84-369">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="e2c84-369">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e2c84-370">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="e2c84-370">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e2c84-371">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-371">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e2c84-372">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-372">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e2c84-373">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-373">`edition`.</span></span> <span data-ttu-id="e2c84-374">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="e2c84-374">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e2c84-375">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-375">`elasticPoolName`.</span></span> <span data-ttu-id="e2c84-376">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="e2c84-376">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e2c84-377">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="e2c84-377">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e2c84-378">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-378">`edition`.</span></span> <span data-ttu-id="e2c84-379">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="e2c84-379">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e2c84-380">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-380">`dtu`.</span></span> <span data-ttu-id="e2c84-381">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="e2c84-381">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e2c84-382">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-382">`databaseDtuMin`.</span></span> <span data-ttu-id="e2c84-383">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="e2c84-383">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e2c84-384">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-384">`databaseDtuMax`.</span></span> <span data-ttu-id="e2c84-385">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="e2c84-385">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e2c84-386">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="e2c84-386">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e2c84-387">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="e2c84-387">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-388">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-388">Storage</span></span>

* <span data-ttu-id="e2c84-389">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-389">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e2c84-390">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="e2c84-390">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-391">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-391">VM</span></span>

* <span data-ttu-id="e2c84-392">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-392">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e2c84-393">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="e2c84-393">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e2c84-394">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="e2c84-394">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e2c84-395">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="e2c84-395">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e2c84-396">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-396">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e2c84-397">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-397">May 7, 2018</span></span>

<span data-ttu-id="e2c84-398">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e2c84-398">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-399">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-399">Core</span></span>

* <span data-ttu-id="e2c84-400">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="e2c84-400">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e2c84-401">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="e2c84-401">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e2c84-402">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-402">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e2c84-403">#5591</span><span class="sxs-lookup"><span data-stu-id="e2c84-403">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e2c84-404">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-404">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e2c84-405">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="e2c84-405">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e2c84-406">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-406">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e2c84-407">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="e2c84-407">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e2c84-408">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-408">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-409">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-409">ACR</span></span>

* <span data-ttu-id="e2c84-410">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-410">Added ACR Build commands</span></span>
* <span data-ttu-id="e2c84-411">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="e2c84-411">Improved resource not found error messages</span></span>
* <span data-ttu-id="e2c84-412">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-412">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e2c84-413">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="e2c84-413">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e2c84-414">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="e2c84-414">Improved repository commands error messages</span></span>
* <span data-ttu-id="e2c84-415">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="e2c84-415">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-416">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-416">ACS</span></span>

* <span data-ttu-id="e2c84-417">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="e2c84-417">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e2c84-418">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="e2c84-418">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e2c84-419">AMS</span><span class="sxs-lookup"><span data-stu-id="e2c84-419">AMS</span></span>

* <span data-ttu-id="e2c84-420">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="e2c84-420">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-421">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-421">Appservice</span></span>

* <span data-ttu-id="e2c84-422">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="e2c84-422">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e2c84-423">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-423">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e2c84-424">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="e2c84-424">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e2c84-425">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-425">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e2c84-426">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-426">Batch AI</span></span>

* <span data-ttu-id="e2c84-427">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="e2c84-427">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e2c84-428">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e2c84-428">Cognitive Services</span></span>

* <span data-ttu-id="e2c84-429">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="e2c84-429">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e2c84-430">Consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-430">Consumption</span></span>

* <span data-ttu-id="e2c84-431">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="e2c84-431">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-432">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-432">Container</span></span>

* <span data-ttu-id="e2c84-433">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="e2c84-433">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e2c84-434">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e2c84-434">Cosmos DB</span></span>

* <span data-ttu-id="e2c84-435">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e2c84-435">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e2c84-436">DMS</span><span class="sxs-lookup"><span data-stu-id="e2c84-436">DMS</span></span>

* <span data-ttu-id="e2c84-437">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="e2c84-437">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-438">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-438">Extension</span></span>

* <span data-ttu-id="e2c84-439">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="e2c84-439">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-440">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-440">Interactive</span></span>

* <span data-ttu-id="e2c84-441">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="e2c84-441">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e2c84-442">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="e2c84-442">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e2c84-443">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="e2c84-443">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e2c84-444">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-444">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e2c84-445">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-445">Lab</span></span>

* <span data-ttu-id="e2c84-446">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="e2c84-446">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-447">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-447">Network</span></span>

* <span data-ttu-id="e2c84-448">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="e2c84-448">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e2c84-449">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-449">Profile</span></span>

* <span data-ttu-id="e2c84-450">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-450">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e2c84-451">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="e2c84-451">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e2c84-452">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="e2c84-452">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e2c84-453">Redis</span><span class="sxs-lookup"><span data-stu-id="e2c84-453">Redis</span></span>

* <span data-ttu-id="e2c84-454">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-454">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e2c84-455">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="e2c84-455">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e2c84-456">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-456">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e2c84-457">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="e2c84-457">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e2c84-458">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-458">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-459">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-459">Role</span></span>

* <span data-ttu-id="e2c84-460">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e2c84-460">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-461">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-461">Storage</span></span>

* <span data-ttu-id="e2c84-462">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="e2c84-462">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e2c84-463">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="e2c84-463">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e2c84-464">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="e2c84-464">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e2c84-465">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="e2c84-465">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e2c84-466">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-466">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-467">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-467">VM</span></span>

* <span data-ttu-id="e2c84-468">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="e2c84-468">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e2c84-469">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e2c84-469">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e2c84-470">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="e2c84-470">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e2c84-471">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="e2c84-471">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e2c84-472">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="e2c84-472">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e2c84-473">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="e2c84-473">Added write accelerator support</span></span>
* <span data-ttu-id="e2c84-474">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e2c84-474">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e2c84-475">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-475">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e2c84-476">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="e2c84-476">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e2c84-477">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-477">April 10, 2018</span></span>

<span data-ttu-id="e2c84-478">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e2c84-478">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-479">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-479">ACR</span></span>

* <span data-ttu-id="e2c84-480">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="e2c84-480">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-481">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-481">ACS</span></span>

* <span data-ttu-id="e2c84-482">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="e2c84-482">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-483">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-483">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e2c84-485">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="e2c84-485">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e2c84-486">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-486">BatchAI</span></span>

* <span data-ttu-id="e2c84-487">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="e2c84-487">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="e2c84-488">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-488">Job level mounting</span></span>
 - <span data-ttu-id="e2c84-489">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="e2c84-489">Environment variables with secret values</span></span>
 - <span data-ttu-id="e2c84-490">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="e2c84-490">Performance counters settings</span></span>
 - <span data-ttu-id="e2c84-491">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-491">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="e2c84-492">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="e2c84-492">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="e2c84-493">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="e2c84-493">Usage and limits reporting</span></span>
 - <span data-ttu-id="e2c84-494">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="e2c84-494">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="e2c84-495">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="e2c84-495">Support for custom images</span></span>
 - <span data-ttu-id="e2c84-496">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="e2c84-496">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e2c84-497">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-497">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e2c84-498">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="e2c84-498">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e2c84-499">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="e2c84-499">National clouds are supported</span></span>
* <span data-ttu-id="e2c84-500">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="e2c84-500">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e2c84-501">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="e2c84-501">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e2c84-502">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-502">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e2c84-503">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="e2c84-503">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e2c84-504">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="e2c84-504">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e2c84-505">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="e2c84-505">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e2c84-506">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-506">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e2c84-507">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="e2c84-507">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e2c84-508">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="e2c84-508">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e2c84-509">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-509">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e2c84-510">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-510">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e2c84-511">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="e2c84-511">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e2c84-512">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-512">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e2c84-513">Facturation</span><span class="sxs-lookup"><span data-stu-id="e2c84-513">Billing</span></span>

* <span data-ttu-id="e2c84-514">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="e2c84-514">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e2c84-515">Consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-515">Consumption</span></span>

* <span data-ttu-id="e2c84-516">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="e2c84-516">Added `marketplace` commands</span></span>
* <span data-ttu-id="e2c84-517">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e2c84-517">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e2c84-518">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="e2c84-518">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e2c84-519">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="e2c84-519">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e2c84-520">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e2c84-520">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e2c84-521">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="e2c84-521">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-522">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-522">Container</span></span>

* <span data-ttu-id="e2c84-523">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="e2c84-523">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e2c84-524">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="e2c84-524">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-525">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-525">Extension</span></span>

* <span data-ttu-id="e2c84-526">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="e2c84-526">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-527">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-527">Interactive</span></span>

* <span data-ttu-id="e2c84-528">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="e2c84-528">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e2c84-529">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-529">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e2c84-530">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="e2c84-530">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-531">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-531">Network</span></span>

* <span data-ttu-id="e2c84-532">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="e2c84-532">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e2c84-533">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-533">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e2c84-534">#4910</span><span class="sxs-lookup"><span data-stu-id="e2c84-534">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e2c84-535">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="e2c84-535">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e2c84-536">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="e2c84-536">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e2c84-537">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-537">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e2c84-538">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-538">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e2c84-539">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="e2c84-539">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-540">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-540">Profile</span></span>

* <span data-ttu-id="e2c84-541">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-541">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e2c84-542">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="e2c84-542">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e2c84-543">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e2c84-543">RDBMS</span></span>

* <span data-ttu-id="e2c84-544">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="e2c84-544">Added `georestore` command</span></span>
* <span data-ttu-id="e2c84-545">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-545">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-546">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-546">Resource</span></span>

* <span data-ttu-id="e2c84-547">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-547">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e2c84-548">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-548">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-549">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-549">SQL</span></span>

* <span data-ttu-id="e2c84-550">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="e2c84-550">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-551">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-551">Storage</span></span>

* <span data-ttu-id="e2c84-552">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="e2c84-552">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-553">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-553">VM</span></span>

* <span data-ttu-id="e2c84-554">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-554">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e2c84-555">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="e2c84-555">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e2c84-557">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-557">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e2c84-558">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="e2c84-558">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e2c84-559">#5718</span><span class="sxs-lookup"><span data-stu-id="e2c84-559">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e2c84-560">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="e2c84-560">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e2c84-561">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-561">March 27, 2018</span></span>

<span data-ttu-id="e2c84-562">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e2c84-562">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-563">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-563">Core</span></span>

* <span data-ttu-id="e2c84-564">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="e2c84-564">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-565">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-565">ACS</span></span>

* <span data-ttu-id="e2c84-566">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e2c84-566">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-567">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-567">Appservice</span></span>

* <span data-ttu-id="e2c84-568">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-568">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e2c84-569">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-569">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e2c84-570">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e2c84-570">Backup</span></span>

* <span data-ttu-id="e2c84-571">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="e2c84-571">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e2c84-572">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-572">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e2c84-573">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e2c84-573">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="e2c84-574">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-574">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-575">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-575">Container</span></span>

* <span data-ttu-id="e2c84-576">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="e2c84-576">Added `container exec` command.</span></span> <span data-ttu-id="e2c84-577">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="e2c84-577">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e2c84-578">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-578">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-579">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-579">Extension</span></span>

* <span data-ttu-id="e2c84-580">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="e2c84-580">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e2c84-581">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e2c84-581">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e2c84-582">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-582">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-583">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-583">Interactive</span></span>

* <span data-ttu-id="e2c84-584">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-584">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e2c84-585">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="e2c84-585">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e2c84-586">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="e2c84-586">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e2c84-587">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="e2c84-587">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e2c84-588">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-588">Lab</span></span>

* <span data-ttu-id="e2c84-589">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="e2c84-589">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-590">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-590">Monitor</span></span>

* <span data-ttu-id="e2c84-591">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e2c84-591">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e2c84-592">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="e2c84-592">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e2c84-593">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e2c84-593">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-594">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-594">Network</span></span>

* <span data-ttu-id="e2c84-595">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="e2c84-595">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-596">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-596">Profile</span></span>

* <span data-ttu-id="e2c84-597">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="e2c84-597">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e2c84-598">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e2c84-598">RDBMS</span></span>

* <span data-ttu-id="e2c84-599">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e2c84-599">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-600">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-600">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e2c84-602">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-602">Role</span></span>

* <span data-ttu-id="e2c84-603">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-603">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e2c84-604">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="e2c84-604">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e2c84-605">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-605">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e2c84-606">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-606">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e2c84-607">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="e2c84-607">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-608">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-608">Storage</span></span>

* <span data-ttu-id="e2c84-609">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="e2c84-609">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e2c84-610">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="e2c84-610">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-611">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-611">VM</span></span>

* <span data-ttu-id="e2c84-612">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="e2c84-612">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e2c84-613">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-613">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e2c84-614">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="e2c84-614">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e2c84-615">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="e2c84-615">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e2c84-616">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-616">March 13, 2018</span></span>

<span data-ttu-id="e2c84-617">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e2c84-617">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-618">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-618">ACR</span></span>

* <span data-ttu-id="e2c84-619">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e2c84-619">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e2c84-620">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="e2c84-620">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e2c84-621">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="e2c84-621">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-622">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-622">ACS</span></span>

* <span data-ttu-id="e2c84-623">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="e2c84-623">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e2c84-624">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="e2c84-624">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e2c84-625">Advisor</span><span class="sxs-lookup"><span data-stu-id="e2c84-625">Advisor</span></span>

* <span data-ttu-id="e2c84-626">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-626">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e2c84-627">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-627">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e2c84-628">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="e2c84-628">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e2c84-629">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-629">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e2c84-630">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-630">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-631">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-631">Appservice</span></span>

* <span data-ttu-id="e2c84-632">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="e2c84-632">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e2c84-633">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-633">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e2c84-634">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="e2c84-634">Eventhubs</span></span>

* <span data-ttu-id="e2c84-635">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-635">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-636">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-636">Extension</span></span>

* <span data-ttu-id="e2c84-637">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-637">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-638">Interactive</span></span>

* <span data-ttu-id="e2c84-639">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="e2c84-639">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e2c84-640">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="e2c84-640">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e2c84-641">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="e2c84-641">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e2c84-642">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="e2c84-642">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-643">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-643">Monitor</span></span>

* <span data-ttu-id="e2c84-644">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="e2c84-644">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e2c84-645">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e2c84-645">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e2c84-646">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e2c84-646">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e2c84-647">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e2c84-647">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-648">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-648">Network</span></span>

* <span data-ttu-id="e2c84-649">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-649">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e2c84-650">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e2c84-650">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e2c84-651">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="e2c84-651">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e2c84-652">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e2c84-652">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-653">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-653">Profile</span></span>

* <span data-ttu-id="e2c84-654">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="e2c84-654">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e2c84-655">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="e2c84-655">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e2c84-656">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e2c84-656">RDBMS</span></span>

* <span data-ttu-id="e2c84-657">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="e2c84-657">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e2c84-658">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e2c84-658">Service Bus</span></span>

* <span data-ttu-id="e2c84-659">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-659">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-660">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-660">Storage</span></span>

* <span data-ttu-id="e2c84-661">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="e2c84-661">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e2c84-662">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="e2c84-662">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-663">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-663">VM</span></span>

* <span data-ttu-id="e2c84-664">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="e2c84-664">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e2c84-665">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="e2c84-665">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e2c84-666">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="e2c84-666">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e2c84-667">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="e2c84-667">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e2c84-668">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-668">February 27, 2018</span></span>

<span data-ttu-id="e2c84-669">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e2c84-669">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-670">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-670">Core</span></span>

* <span data-ttu-id="e2c84-671">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="e2c84-671">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e2c84-672">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="e2c84-672">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e2c84-673">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="e2c84-673">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-674">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-674">ACS</span></span>

* <span data-ttu-id="e2c84-675">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-675">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e2c84-676">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="e2c84-676">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e2c84-677">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e2c84-677">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e2c84-678">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-678">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-679">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-679">Appservice</span></span>

* <span data-ttu-id="e2c84-680">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e2c84-680">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e2c84-681">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="e2c84-681">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e2c84-682">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e2c84-682">Cognitive Services</span></span>

* <span data-ttu-id="e2c84-683">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e2c84-683">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e2c84-684">Consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-684">Consumption</span></span>

* <span data-ttu-id="e2c84-685">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="e2c84-685">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e2c84-686">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="e2c84-686">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-687">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-687">Container</span></span>

* <span data-ttu-id="e2c84-688">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="e2c84-688">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-689">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-689">Network</span></span>

* <span data-ttu-id="e2c84-690">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e2c84-690">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-691">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-691">Resource</span></span>

* <span data-ttu-id="e2c84-692">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="e2c84-692">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-693">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-693">Role</span></span>

* <span data-ttu-id="e2c84-694">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="e2c84-694">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-695">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-695">SQL</span></span>

* <span data-ttu-id="e2c84-696">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="e2c84-696">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-697">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-697">Storage</span></span>

* <span data-ttu-id="e2c84-698">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-698">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-699">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-699">VM</span></span>

* <span data-ttu-id="e2c84-700">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="e2c84-700">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e2c84-701">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-701">February 13, 2018</span></span>

<span data-ttu-id="e2c84-702">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e2c84-702">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-703">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-703">Core</span></span>

* <span data-ttu-id="e2c84-704">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="e2c84-704">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-705">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-705">ACS</span></span>

* <span data-ttu-id="e2c84-706">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="e2c84-706">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e2c84-707">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-707">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e2c84-708">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e2c84-708">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e2c84-709">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="e2c84-709">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e2c84-710">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="e2c84-710">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e2c84-711">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e2c84-711">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e2c84-712">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e2c84-712">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e2c84-713">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e2c84-713">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-714">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-714">Appservice</span></span>

* <span data-ttu-id="e2c84-715">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="e2c84-715">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e2c84-716">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e2c84-716">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e2c84-717">CDN</span><span class="sxs-lookup"><span data-stu-id="e2c84-717">CDN</span></span>

* <span data-ttu-id="e2c84-718">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-718">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-719">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-719">Container</span></span>

* <span data-ttu-id="e2c84-720">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="e2c84-720">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e2c84-721">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-721">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e2c84-722">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e2c84-722">CosmosDB</span></span>

* <span data-ttu-id="e2c84-723">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="e2c84-723">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-724">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-724">Extension</span></span>

* <span data-ttu-id="e2c84-725">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-725">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e2c84-726">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-726">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e2c84-727">Commentaires</span><span class="sxs-lookup"><span data-stu-id="e2c84-727">Feedback</span></span>

* <span data-ttu-id="e2c84-728">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="e2c84-728">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-729">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-729">Interactive</span></span>

* <span data-ttu-id="e2c84-730">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e2c84-730">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e2c84-731">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="e2c84-731">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-732">IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-732">IoT</span></span>

* <span data-ttu-id="e2c84-733">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="e2c84-733">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e2c84-734">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="e2c84-734">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e2c84-735">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-735">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e2c84-736">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="e2c84-736">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-737">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-737">Monitor</span></span>

* <span data-ttu-id="e2c84-738">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-738">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-739">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-739">Network</span></span>

* <span data-ttu-id="e2c84-740">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e2c84-740">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e2c84-741">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-741">Profile</span></span>

* <span data-ttu-id="e2c84-742">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="e2c84-742">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-743">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-743">Resource</span></span>

* <span data-ttu-id="e2c84-744">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-744">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-745">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-745">Role</span></span>

* <span data-ttu-id="e2c84-746">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-746">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-747">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-747">SQL</span></span>

* <span data-ttu-id="e2c84-748">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e2c84-748">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e2c84-749">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e2c84-749">Added `sql db rename`</span></span>
* <span data-ttu-id="e2c84-750">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="e2c84-750">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-751">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-751">Storage</span></span>

* <span data-ttu-id="e2c84-752">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="e2c84-752">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-753">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-753">VM</span></span>

* <span data-ttu-id="e2c84-754">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="e2c84-754">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e2c84-755">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="e2c84-755">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e2c84-756">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="e2c84-756">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e2c84-757">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-757">January 31, 2018</span></span>

<span data-ttu-id="e2c84-758">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e2c84-758">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-759">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-759">Core</span></span>

* <span data-ttu-id="e2c84-760">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="e2c84-760">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e2c84-761">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="e2c84-761">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e2c84-762">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="e2c84-762">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e2c84-763">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="e2c84-763">Use `--verbose` to see</span></span>
* <span data-ttu-id="e2c84-764">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="e2c84-764">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-765">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-765">ACS</span></span>

* <span data-ttu-id="e2c84-766">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="e2c84-766">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e2c84-767">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e2c84-767">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-768">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-768">Appservice</span></span>

* <span data-ttu-id="e2c84-769">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="e2c84-769">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e2c84-770">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="e2c84-770">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e2c84-771">CDN</span><span class="sxs-lookup"><span data-stu-id="e2c84-771">CDN</span></span>

* <span data-ttu-id="e2c84-772">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-772">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e2c84-773">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e2c84-773">CosmosDB</span></span>

* <span data-ttu-id="e2c84-774">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="e2c84-774">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-775">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-775">Interactive</span></span>

* <span data-ttu-id="e2c84-776">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="e2c84-776">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-777">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-777">Network</span></span>

* <span data-ttu-id="e2c84-778">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-778">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e2c84-779">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-779">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e2c84-780">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-780">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e2c84-781">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-781">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e2c84-782">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e2c84-782">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e2c84-783">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="e2c84-783">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e2c84-784">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="e2c84-784">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e2c84-785">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="e2c84-785">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e2c84-786">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e2c84-786">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e2c84-787">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e2c84-787">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-788">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-788">Profile</span></span>

* <span data-ttu-id="e2c84-789">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="e2c84-789">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-790">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-790">Resource</span></span>

* <span data-ttu-id="e2c84-791">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="e2c84-791">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-792">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-792">Storage</span></span>

* <span data-ttu-id="e2c84-793">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="e2c84-793">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e2c84-794">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="e2c84-794">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e2c84-795">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-795">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e2c84-796">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-796">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e2c84-797">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="e2c84-797">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-798">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-798">VM</span></span>

* <span data-ttu-id="e2c84-799">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="e2c84-799">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e2c84-800">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="e2c84-800">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e2c84-801">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="e2c84-801">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e2c84-802">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-802">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e2c84-803">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="e2c84-803">January 17, 2018</span></span>

<span data-ttu-id="e2c84-804">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e2c84-804">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-805">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-805">ACR</span></span>

* <span data-ttu-id="e2c84-806">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="e2c84-806">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e2c84-807">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="e2c84-807">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-808">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-808">ACS</span></span>

* <span data-ttu-id="e2c84-809">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e2c84-809">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e2c84-810">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="e2c84-810">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-811">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-811">Appservice</span></span>

* <span data-ttu-id="e2c84-812">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="e2c84-812">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e2c84-813">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="e2c84-813">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e2c84-814">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="e2c84-814">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e2c84-815">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e2c84-815">Backup</span></span>

* <span data-ttu-id="e2c84-816">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="e2c84-816">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e2c84-817">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e2c84-817">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e2c84-818">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="e2c84-818">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e2c84-819">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="e2c84-819">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e2c84-820">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-820">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-821">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-821">Batch</span></span>

* <span data-ttu-id="e2c84-822">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="e2c84-822">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e2c84-823">Cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-823">Cloud</span></span>

* <span data-ttu-id="e2c84-824">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-824">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e2c84-825">Consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-825">Consumption</span></span>

* <span data-ttu-id="e2c84-826">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e2c84-826">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e2c84-827">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e2c84-827">Event Grid</span></span>

* <span data-ttu-id="e2c84-828">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e2c84-828">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e2c84-829">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e2c84-829">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e2c84-830">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e2c84-830">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e2c84-831">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="e2c84-831">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e2c84-832">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-832">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e2c84-833">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-833">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e2c84-834">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e2c84-834">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e2c84-835">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="e2c84-835">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-836">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-836">Interactive</span></span>

* <span data-ttu-id="e2c84-837">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e2c84-837">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e2c84-838">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="e2c84-838">Fixed errors on startup</span></span>
* <span data-ttu-id="e2c84-839">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="e2c84-839">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-840">IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-840">IoT</span></span>

* <span data-ttu-id="e2c84-841">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="e2c84-841">Added support for device provisioning service</span></span>
* <span data-ttu-id="e2c84-842">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-842">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e2c84-843">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-843">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-844">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-844">Monitor</span></span>

* <span data-ttu-id="e2c84-845">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="e2c84-845">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e2c84-846">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-846">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e2c84-847">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="e2c84-847">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-848">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-848">Network</span></span>

* <span data-ttu-id="e2c84-849">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-849">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e2c84-850">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-850">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-851">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-851">Profile</span></span>

* <span data-ttu-id="e2c84-852">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-852">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-853">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-853">Role</span></span>

* <span data-ttu-id="e2c84-854">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="e2c84-854">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e2c84-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e2c84-855">Service Fabric</span></span>

* <span data-ttu-id="e2c84-856">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="e2c84-856">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e2c84-857">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-857">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-858">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-858">VM</span></span>

* <span data-ttu-id="e2c84-859">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="e2c84-859">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e2c84-860">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="e2c84-860">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e2c84-861">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="e2c84-861">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e2c84-862">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="e2c84-862">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e2c84-863">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="e2c84-863">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e2c84-864">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-864">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e2c84-865">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-865">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e2c84-866">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e2c84-866">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e2c84-867">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-867">December 19, 2017</span></span>

<span data-ttu-id="e2c84-868">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e2c84-868">Version 2.0.23</span></span>

* <span data-ttu-id="e2c84-869">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-869">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-870">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-870">Container</span></span>

* <span data-ttu-id="e2c84-871">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-871">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-872">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-872">Network</span></span>

* <span data-ttu-id="e2c84-873">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-873">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e2c84-874">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-874">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-875">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-875">Storage</span></span>

* <span data-ttu-id="e2c84-876">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="e2c84-876">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-877">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-877">VM</span></span>

* <span data-ttu-id="e2c84-878">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="e2c84-878">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e2c84-879">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-879">December 5, 2017</span></span>

<span data-ttu-id="e2c84-880">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e2c84-880">Version 2.0.22</span></span>

* <span data-ttu-id="e2c84-881">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-881">Removed `az component` commands.</span></span> <span data-ttu-id="e2c84-882">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="e2c84-882">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-883">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-883">Core</span></span>
* <span data-ttu-id="e2c84-884">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e2c84-884">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e2c84-885">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="e2c84-885">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-886">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-886">ACS</span></span>

* <span data-ttu-id="e2c84-887">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e2c84-887">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e2c84-888">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-888">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e2c84-889">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="e2c84-889">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e2c84-890">Advisor</span><span class="sxs-lookup"><span data-stu-id="e2c84-890">Advisor</span></span>

* <span data-ttu-id="e2c84-891">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-891">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-892">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-892">Appservice</span></span>

* <span data-ttu-id="e2c84-893">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e2c84-893">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e2c84-894">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="e2c84-894">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e2c84-895">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e2c84-895">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e2c84-896">Consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-896">Consumption</span></span>

* <span data-ttu-id="e2c84-897">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="e2c84-897">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-898">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-898">Container</span></span>

* <span data-ttu-id="e2c84-899">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-899">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-900">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-900">Monitor</span></span>

* <span data-ttu-id="e2c84-901">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="e2c84-901">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-902">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-902">Resource</span></span>

* <span data-ttu-id="e2c84-903">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-903">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-904">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-904">Role</span></span>

* <span data-ttu-id="e2c84-905">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-905">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e2c84-906">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="e2c84-906">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e2c84-907">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e2c84-907">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-908">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-908">SQL</span></span>

* <span data-ttu-id="e2c84-909">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="e2c84-909">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e2c84-910">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-910">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-911">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-911">VM</span></span>

* <span data-ttu-id="e2c84-912">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e2c84-912">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e2c84-913">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-913">November 14, 2017</span></span>

<span data-ttu-id="e2c84-914">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e2c84-914">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-915">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-915">ACR</span></span>

* <span data-ttu-id="e2c84-916">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="e2c84-916">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e2c84-917">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-917">ACS</span></span>

* <span data-ttu-id="e2c84-918">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="e2c84-918">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e2c84-919">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-919">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e2c84-920">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e2c84-920">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e2c84-921">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="e2c84-921">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e2c84-922">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="e2c84-922">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-923">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-923">Appservice</span></span>

* <span data-ttu-id="e2c84-924">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="e2c84-924">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e2c84-925">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e2c84-925">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e2c84-926">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e2c84-926">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e2c84-927">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e2c84-927">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e2c84-928">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="e2c84-928">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e2c84-929">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="e2c84-929">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-930">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-930">Batch</span></span>

* <span data-ttu-id="e2c84-931">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="e2c84-931">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e2c84-932">Batchai</span><span class="sxs-lookup"><span data-stu-id="e2c84-932">Batchai</span></span>

* <span data-ttu-id="e2c84-933">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-933">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e2c84-934">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-934">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e2c84-935">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e2c84-935">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e2c84-936">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-936">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e2c84-937">Cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-937">Cloud</span></span>

* <span data-ttu-id="e2c84-938">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="e2c84-938">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-939">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-939">Container</span></span>

* <span data-ttu-id="e2c84-940">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="e2c84-940">Added support to open multiple ports</span></span>
* <span data-ttu-id="e2c84-941">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="e2c84-941">Added container group restart policy</span></span>
* <span data-ttu-id="e2c84-942">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="e2c84-942">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e2c84-943">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="e2c84-943">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e2c84-944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e2c84-944">Data Lake Analytics</span></span>

* <span data-ttu-id="e2c84-945">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="e2c84-945">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e2c84-946">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-946">Data Lake Store</span></span>

* <span data-ttu-id="e2c84-947">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="e2c84-947">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-948">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-948">Extension</span></span>

* <span data-ttu-id="e2c84-949">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="e2c84-949">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e2c84-950">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="e2c84-950">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-951">IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-951">IoT</span></span>

* <span data-ttu-id="e2c84-952">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="e2c84-952">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-953">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-953">Monitor</span></span>

* <span data-ttu-id="e2c84-954">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e2c84-954">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-955">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-955">Network</span></span>

* <span data-ttu-id="e2c84-956">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="e2c84-956">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e2c84-957">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-957">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e2c84-958">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="e2c84-958">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e2c84-959">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e2c84-959">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e2c84-960">Réservations</span><span class="sxs-lookup"><span data-stu-id="e2c84-960">Reservations</span></span>

* <span data-ttu-id="e2c84-961">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-961">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-962">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-962">Resource</span></span>

* <span data-ttu-id="e2c84-963">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="e2c84-963">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-964">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-964">SQL</span></span>

* <span data-ttu-id="e2c84-965">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-965">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-966">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-966">Storage</span></span>

* <span data-ttu-id="e2c84-967">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-967">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e2c84-968">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="e2c84-968">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e2c84-969">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e2c84-969">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e2c84-970">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e2c84-970">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e2c84-971">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-971">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e2c84-972">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e2c84-972">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e2c84-973">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-973">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-974">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-974">VM</span></span>

* <span data-ttu-id="e2c84-975">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="e2c84-975">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e2c84-976">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="e2c84-976">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e2c84-977">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="e2c84-977">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e2c84-978">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e2c84-978">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e2c84-979">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e2c84-979">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e2c84-980">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-980">October 24, 2017</span></span>

<span data-ttu-id="e2c84-981">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e2c84-981">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-982">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-982">Core</span></span>

* <span data-ttu-id="e2c84-983">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e2c84-983">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-984">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-984">ACR</span></span>

* <span data-ttu-id="e2c84-985">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e2c84-985">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e2c84-986">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="e2c84-986">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e2c84-987">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="e2c84-987">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-988">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-988">ACS</span></span>

* <span data-ttu-id="e2c84-989">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="e2c84-989">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e2c84-990">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e2c84-990">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-991">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-991">Appservice</span></span>

* <span data-ttu-id="e2c84-992">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="e2c84-992">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e2c84-993">Composant</span><span class="sxs-lookup"><span data-stu-id="e2c84-993">Component</span></span>

* <span data-ttu-id="e2c84-994">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="e2c84-994">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-995">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-995">Monitor</span></span>

* <span data-ttu-id="e2c84-996">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="e2c84-996">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-997">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-997">Resource</span></span>

* <span data-ttu-id="e2c84-998">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="e2c84-998">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e2c84-999">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="e2c84-999">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1000">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1000">VM</span></span>

* <span data-ttu-id="e2c84-1001">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1001">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e2c84-1002">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1002">October 9, 2017</span></span>

<span data-ttu-id="e2c84-1003">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e2c84-1003">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-1004">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-1004">Core</span></span>

* <span data-ttu-id="e2c84-1005">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e2c84-1005">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1006">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1006">Appservice</span></span>

* <span data-ttu-id="e2c84-1007">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1007">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-1008">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-1008">Batch</span></span>

* <span data-ttu-id="e2c84-1009">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e2c84-1009">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e2c84-1010">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="e2c84-1010">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e2c84-1011">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-1011">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e2c84-1012">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="e2c84-1012">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e2c84-1013">Batchai</span><span class="sxs-lookup"><span data-stu-id="e2c84-1013">Batchai</span></span>

* <span data-ttu-id="e2c84-1014">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="e2c84-1014">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-1015">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-1015">Keyvault</span></span>

* <span data-ttu-id="e2c84-1016">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1016">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e2c84-1017">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1017">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e2c84-1018">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1018">Network</span></span>

* <span data-ttu-id="e2c84-1019">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="e2c84-1019">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e2c84-1020">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="e2c84-1020">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-1021">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-1021">Resource</span></span>

* <span data-ttu-id="e2c84-1022">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1022">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e2c84-1023">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1023">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e2c84-1024">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="e2c84-1024">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e2c84-1025">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="e2c84-1025">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-1026">Sql</span></span>

* <span data-ttu-id="e2c84-1027">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="e2c84-1027">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e2c84-1028">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="e2c84-1028">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e2c84-1029">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="e2c84-1029">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1030">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1030">Storage</span></span>

* <span data-ttu-id="e2c84-1031">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="e2c84-1031">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1032">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1032">Vm</span></span>

* <span data-ttu-id="e2c84-1033">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="e2c84-1033">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e2c84-1034">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1034">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e2c84-1035">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1035">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e2c84-1036">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1036">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e2c84-1037">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1037">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e2c84-1038">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1038">September 22, 2017</span></span>

<span data-ttu-id="e2c84-1039">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e2c84-1039">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-1040">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-1040">Resource</span></span>

* <span data-ttu-id="e2c84-1041">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1041">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e2c84-1042">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="e2c84-1042">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e2c84-1043">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1043">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e2c84-1044">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1044">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1045">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1045">Network</span></span>

* <span data-ttu-id="e2c84-1046">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1046">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e2c84-1047">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1047">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e2c84-1048">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1048">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e2c84-1049">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1049">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e2c84-1050">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1050">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e2c84-1051">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1051">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e2c84-1052">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1052">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1053">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1053">Storage</span></span>

* <span data-ttu-id="e2c84-1054">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1054">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e2c84-1055">Événement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1055">Eventgrid</span></span>

* <span data-ttu-id="e2c84-1056">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="e2c84-1056">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-1057">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-1057">SQL</span></span>

* <span data-ttu-id="e2c84-1058">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1058">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e2c84-1059">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1059">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e2c84-1060">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1060">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-1061">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-1061">Keyvault</span></span>

* <span data-ttu-id="e2c84-1062">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="e2c84-1062">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1063">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1063">VM</span></span>

* <span data-ttu-id="e2c84-1064">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1064">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e2c84-1065">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="e2c84-1065">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e2c84-1066">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1066">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e2c84-1067">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1067">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e2c84-1068">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1068">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e2c84-1069">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1069">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1070">ACS</span></span>

* <span data-ttu-id="e2c84-1071">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="e2c84-1071">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1072">Appservice</span></span>

* <span data-ttu-id="e2c84-1073">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1073">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e2c84-1074">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="e2c84-1074">Backup</span></span>

* <span data-ttu-id="e2c84-1075">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1075">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e2c84-1076">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1076">September 11, 2017</span></span>

<span data-ttu-id="e2c84-1077">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e2c84-1077">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e2c84-1078">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-1078">Core</span></span>

* <span data-ttu-id="e2c84-1079">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="e2c84-1079">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e2c84-1080">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="e2c84-1080">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1081">Acs</span><span class="sxs-lookup"><span data-stu-id="e2c84-1081">Acs</span></span>

* <span data-ttu-id="e2c84-1082">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1082">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e2c84-1083">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="e2c84-1083">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1084">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1084">Appservice</span></span>

* <span data-ttu-id="e2c84-1085">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="e2c84-1085">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e2c84-1086">CDN</span><span class="sxs-lookup"><span data-stu-id="e2c84-1086">CDN</span></span>

* <span data-ttu-id="e2c84-1087">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1087">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e2c84-1088">Extension</span><span class="sxs-lookup"><span data-stu-id="e2c84-1088">Extension</span></span>

* <span data-ttu-id="e2c84-1089">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-1089">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-1090">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-1090">Keyvault</span></span>

* <span data-ttu-id="e2c84-1091">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1091">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1092">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1092">Network</span></span>

* <span data-ttu-id="e2c84-1093">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1093">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e2c84-1094">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1094">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e2c84-1095">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1095">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e2c84-1096">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1096">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e2c84-1097">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1097">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-1098">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-1098">Resource</span></span>

* <span data-ttu-id="e2c84-1099">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1099">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e2c84-1100">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1100">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e2c84-1101">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="e2c84-1101">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e2c84-1102">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="e2c84-1102">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-1103">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-1103">SQL</span></span>

* <span data-ttu-id="e2c84-1104">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1104">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1105">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1105">VM</span></span>

* <span data-ttu-id="e2c84-1106">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="e2c84-1106">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e2c84-1107">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="e2c84-1107">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e2c84-1108">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1108">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e2c84-1109">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="e2c84-1109">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e2c84-1110">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="e2c84-1110">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e2c84-1111">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1111">August 31, 2017</span></span>

<span data-ttu-id="e2c84-1112">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e2c84-1112">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-1113">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-1113">Keyvault</span></span>

* <span data-ttu-id="e2c84-1114">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1114">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e2c84-1115">Sf</span><span class="sxs-lookup"><span data-stu-id="e2c84-1115">Sf</span></span>

* <span data-ttu-id="e2c84-1116">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1116">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1117">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1117">Storage</span></span>

* <span data-ttu-id="e2c84-1118">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="e2c84-1118">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e2c84-1119">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1119">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e2c84-1120">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1120">August 28, 2017</span></span>

<span data-ttu-id="e2c84-1121">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e2c84-1121">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e2c84-1122">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-1122">CLI</span></span>

* <span data-ttu-id="e2c84-1123">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1123">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1124">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1124">ACS</span></span>

* <span data-ttu-id="e2c84-1125">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="e2c84-1125">Corrected preview regions</span></span>
* <span data-ttu-id="e2c84-1126">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1126">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e2c84-1127">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1127">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1128">Appservice</span></span>

* <span data-ttu-id="e2c84-1129">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1129">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e2c84-1130">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1130">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e2c84-1131">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1131">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e2c84-1132">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1132">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e2c84-1133">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1133">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-1134">IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-1134">IoT</span></span>

* <span data-ttu-id="e2c84-1135">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="e2c84-1135">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1136">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1136">Network</span></span>

* <span data-ttu-id="e2c84-1137">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1137">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e2c84-1138">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1138">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e2c84-1139">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1139">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e2c84-1140">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1140">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e2c84-1141">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1141">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-1142">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-1142">Profile</span></span>

* <span data-ttu-id="e2c84-1143">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1143">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e2c84-1144">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e2c84-1144">Service Fabric</span></span>

* <span data-ttu-id="e2c84-1145">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1145">Preview release</span></span>
* <span data-ttu-id="e2c84-1146">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-1146">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e2c84-1147">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="e2c84-1147">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e2c84-1148">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1148">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1149">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1149">Storage</span></span>

* <span data-ttu-id="e2c84-1150">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="e2c84-1150">Enabled setting blob tier</span></span>
* <span data-ttu-id="e2c84-1151">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="e2c84-1151">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e2c84-1152">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1152">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e2c84-1153">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="e2c84-1153">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e2c84-1154">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1154">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e2c84-1155">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="e2c84-1155">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1156">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1156">VM</span></span>

* <span data-ttu-id="e2c84-1157">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1157">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e2c84-1158">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e2c84-1158">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e2c84-1159">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1159">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e2c84-1160">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="e2c84-1160">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e2c84-1161">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="e2c84-1161">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e2c84-1162">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1162">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e2c84-1163">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1163">August 15, 2017</span></span>

<span data-ttu-id="e2c84-1164">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e2c84-1164">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1165">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1165">ACS</span></span>

* <span data-ttu-id="e2c84-1166">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="e2c84-1166">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1167">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1167">Appservice</span></span>

* <span data-ttu-id="e2c84-1168">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="e2c84-1168">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e2c84-1169">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e2c84-1169">Event Grid</span></span>

* <span data-ttu-id="e2c84-1170">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1170">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e2c84-1171">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1171">August 11, 2017</span></span>

<span data-ttu-id="e2c84-1172">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e2c84-1172">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1173">ACS</span></span>

* <span data-ttu-id="e2c84-1174">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="e2c84-1174">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-1175">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-1175">Batch</span></span>

* <span data-ttu-id="e2c84-1176">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e2c84-1176">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e2c84-1177">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-1177">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e2c84-1178">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="e2c84-1178">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e2c84-1179">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="e2c84-1179">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e2c84-1180">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="e2c84-1180">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e2c84-1181">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="e2c84-1181">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e2c84-1182">Composant</span><span class="sxs-lookup"><span data-stu-id="e2c84-1182">Component</span></span>

* <span data-ttu-id="e2c84-1183">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="e2c84-1183">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e2c84-1184">Conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-1184">Container</span></span>

* <span data-ttu-id="e2c84-1185">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1185">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e2c84-1186">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1186">Data Lake Store</span></span>

* <span data-ttu-id="e2c84-1187">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="e2c84-1187">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e2c84-1188">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e2c84-1188">Event Grid</span></span>

* <span data-ttu-id="e2c84-1189">Version initiale</span><span class="sxs-lookup"><span data-stu-id="e2c84-1189">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1190">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1190">Network</span></span>

* <span data-ttu-id="e2c84-1191">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="e2c84-1191">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e2c84-1192">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1192">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e2c84-1193">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="e2c84-1193">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e2c84-1194">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1194">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-1195">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-1195">Profile</span></span>

* <span data-ttu-id="e2c84-1196">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="e2c84-1196">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1197">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1197">Storage</span></span>

* <span data-ttu-id="e2c84-1198">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="e2c84-1198">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1199">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1199">VM</span></span>

* <span data-ttu-id="e2c84-1200">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="e2c84-1200">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e2c84-1201">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1201">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e2c84-1202">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1202">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e2c84-1203">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="e2c84-1203">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e2c84-1204">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1204">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e2c84-1205">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1205">July 28, 2017</span></span>

<span data-ttu-id="e2c84-1206">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e2c84-1206">Version 2.0.12</span></span>

* <span data-ttu-id="e2c84-1207">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="e2c84-1207">Added container commands</span></span>
* <span data-ttu-id="e2c84-1208">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="e2c84-1208">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="e2c84-1209">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-1209">Core</span></span>

* <span data-ttu-id="e2c84-1210">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="e2c84-1210">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e2c84-1211">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1211">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e2c84-1212">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1212">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e2c84-1213">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1213">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e2c84-1214">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="e2c84-1214">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e2c84-1215">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1215">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e2c84-1216">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1216">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e2c84-1217">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1217">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e2c84-1218">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1218">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e2c84-1219">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1219">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e2c84-1220">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="e2c84-1220">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e2c84-1221">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1221">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e2c84-1222">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="e2c84-1222">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e2c84-1223">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="e2c84-1223">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e2c84-1224">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e2c84-1224">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e2c84-1225">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1225">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e2c84-1226">ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-1226">ACR</span></span>

* <span data-ttu-id="e2c84-1227">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1227">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e2c84-1228">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1228">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e2c84-1229">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1229">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e2c84-1230">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="e2c84-1230">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e2c84-1231">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="e2c84-1231">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e2c84-1232">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="e2c84-1232">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1233">ACS</span></span>

* <span data-ttu-id="e2c84-1234">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e2c84-1234">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1235">Appservice</span></span>

* <span data-ttu-id="e2c84-1236">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="e2c84-1236">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e2c84-1237">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="e2c84-1237">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e2c84-1238">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1238">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e2c84-1239">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1239">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e2c84-1240">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1240">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e2c84-1241">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1241">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e2c84-1242">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1242">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e2c84-1243">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1243">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e2c84-1244">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1244">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e2c84-1245">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1245">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e2c84-1246">Batch</span><span class="sxs-lookup"><span data-stu-id="e2c84-1246">Batch</span></span>

* <span data-ttu-id="e2c84-1247">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="e2c84-1247">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e2c84-1248">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1248">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e2c84-1249">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1249">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e2c84-1250">CDN</span><span class="sxs-lookup"><span data-stu-id="e2c84-1250">CDN</span></span>

* <span data-ttu-id="e2c84-1251">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="e2c84-1251">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e2c84-1252">Cloud</span><span class="sxs-lookup"><span data-stu-id="e2c84-1252">Cloud</span></span>

* <span data-ttu-id="e2c84-1253">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="e2c84-1253">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e2c84-1254">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1254">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e2c84-1255">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="e2c84-1255">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e2c84-1256">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="e2c84-1256">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e2c84-1257">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1257">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e2c84-1258">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e2c84-1258">CosmosDB</span></span>

* <span data-ttu-id="e2c84-1259">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1259">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e2c84-1260">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="e2c84-1260">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e2c84-1261">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e2c84-1261">Data Lake Analytics</span></span>

* <span data-ttu-id="e2c84-1262">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1262">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e2c84-1263">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1263">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e2c84-1264">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1264">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e2c84-1265">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1265">Data Lake Store</span></span>

* <span data-ttu-id="e2c84-1266">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1266">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e2c84-1267">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="e2c84-1267">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e2c84-1268">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1268">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e2c84-1269">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1269">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e2c84-1270">Interactive</span><span class="sxs-lookup"><span data-stu-id="e2c84-1270">Interactive</span></span>

* <span data-ttu-id="e2c84-1271">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="e2c84-1271">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e2c84-1272">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="e2c84-1272">Increased test coverage</span></span>
* <span data-ttu-id="e2c84-1273">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="e2c84-1273">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e2c84-1274">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1274">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e2c84-1275">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1275">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e2c84-1276">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1276">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e2c84-1277">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1277">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e2c84-1278">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1278">Added `--progress` flag</span></span>
* <span data-ttu-id="e2c84-1279">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="e2c84-1279">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e2c84-1280">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1280">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e2c84-1281">IoT</span><span class="sxs-lookup"><span data-stu-id="e2c84-1281">IoT</span></span>

* <span data-ttu-id="e2c84-1282">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1282">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e2c84-1283">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1283">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e2c84-1284">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1284">Key vault</span></span>

* <span data-ttu-id="e2c84-1285">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1285">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e2c84-1286">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1286">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e2c84-1287">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1287">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e2c84-1288">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1288">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e2c84-1289">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1289">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e2c84-1290">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1290">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e2c84-1291">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1291">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e2c84-1292">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1292">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e2c84-1293">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1293">Lab</span></span>

* <span data-ttu-id="e2c84-1294">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1294">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e2c84-1295">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1295">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-1296">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-1296">Monitor</span></span>

* <span data-ttu-id="e2c84-1297">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1297">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e2c84-1298">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1298">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e2c84-1299">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1299">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e2c84-1300">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1300">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e2c84-1301">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1301">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e2c84-1302">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e2c84-1302">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e2c84-1303">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="e2c84-1303">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e2c84-1304">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1304">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e2c84-1305">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1305">`location` no longer required</span></span>
  * <span data-ttu-id="e2c84-1306">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="e2c84-1306">Add name and ID support for target</span></span>
  * <span data-ttu-id="e2c84-1307">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1307">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e2c84-1308">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1308">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e2c84-1309">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="e2c84-1309">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e2c84-1310">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="e2c84-1310">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e2c84-1311">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1311">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e2c84-1312">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1312">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1313">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1313">Network</span></span>

* <span data-ttu-id="e2c84-1314">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1314">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e2c84-1315">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1315">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e2c84-1316">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="e2c84-1316">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e2c84-1317">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="e2c84-1317">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e2c84-1318">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1318">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e2c84-1319">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1319">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e2c84-1320">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1320">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e2c84-1321">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1321">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e2c84-1322">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1322">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e2c84-1323">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1323">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e2c84-1324">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1324">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e2c84-1325">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1325">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e2c84-1326">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1326">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e2c84-1327">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1327">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e2c84-1328">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1328">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e2c84-1329">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1329">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e2c84-1330">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1330">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e2c84-1331">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1331">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e2c84-1332">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1332">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e2c84-1333">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1333">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e2c84-1334">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1334">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e2c84-1335">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-1335">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e2c84-1336">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1336">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e2c84-1337">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e2c84-1337">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e2c84-1338">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e2c84-1338">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e2c84-1339">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e2c84-1339">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e2c84-1340">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="e2c84-1340">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-1341">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-1341">Profile</span></span>

* <span data-ttu-id="e2c84-1342">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1342">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e2c84-1343">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1343">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e2c84-1344">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="e2c84-1344">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e2c84-1345">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="e2c84-1345">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e2c84-1346">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="e2c84-1346">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e2c84-1347">SGBDR</span><span class="sxs-lookup"><span data-stu-id="e2c84-1347">RDBMS</span></span>

* <span data-ttu-id="e2c84-1348">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1348">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e2c84-1349">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1349">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e2c84-1350">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1350">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e2c84-1351">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1351">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-1352">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-1352">Resource</span></span>

* <span data-ttu-id="e2c84-1353">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1353">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e2c84-1354">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e2c84-1354">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e2c84-1355">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e2c84-1355">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e2c84-1356">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="e2c84-1356">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e2c84-1357">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1357">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e2c84-1358">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1358">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e2c84-1359">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1359">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e2c84-1360">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="e2c84-1360">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-1361">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1361">Role</span></span>

* <span data-ttu-id="e2c84-1362">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1362">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e2c84-1363">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1363">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e2c84-1364">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="e2c84-1364">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e2c84-1365">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1365">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e2c84-1366">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1366">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e2c84-1367">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e2c84-1367">Service Fabric</span></span>
* <span data-ttu-id="e2c84-1368">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1368">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e2c84-1369">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1369">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e2c84-1370">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1370">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-1371">SQL</span></span>

* <span data-ttu-id="e2c84-1372">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1372">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e2c84-1373">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1373">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e2c84-1374">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1374">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1375">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1375">Storage</span></span>

* <span data-ttu-id="e2c84-1376">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1376">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e2c84-1377">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="e2c84-1377">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e2c84-1378">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1378">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e2c84-1379">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1379">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e2c84-1380">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1380">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e2c84-1381">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1381">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1382">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1382">VM</span></span>

* <span data-ttu-id="e2c84-1383">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1383">Support configuring nsg</span></span>
* <span data-ttu-id="e2c84-1384">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1384">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e2c84-1385">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="e2c84-1385">Support managed service identities</span></span>
* <span data-ttu-id="e2c84-1386">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1386">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e2c84-1387">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="e2c84-1387">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e2c84-1388">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1388">May 10, 2017</span></span>

<span data-ttu-id="e2c84-1389">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e2c84-1389">Version 2.0.6</span></span>

* <span data-ttu-id="e2c84-1390">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e2c84-1390">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e2c84-1391">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1391">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e2c84-1392">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1392">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e2c84-1393">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e2c84-1393">Include Cognitive Services module</span></span>
* <span data-ttu-id="e2c84-1394">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e2c84-1394">Include Service Fabric module</span></span>
* <span data-ttu-id="e2c84-1395">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1395">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e2c84-1396">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="e2c84-1396">Add support for CDN commands</span></span>
* <span data-ttu-id="e2c84-1397">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="e2c84-1397">Remove Container module</span></span>
* <span data-ttu-id="e2c84-1398">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1398">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e2c84-1399">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1399">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="e2c84-1400">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-1400">Core</span></span>

* <span data-ttu-id="e2c84-1401">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1401">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e2c84-1402">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1402">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e2c84-1403">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1403">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e2c84-1404">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1404">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e2c84-1405">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1405">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e2c84-1406">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1406">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e2c84-1407">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1407">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e2c84-1408">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1408">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e2c84-1409">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1409">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e2c84-1410">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="e2c84-1410">core: Improved performance</span></span>
* <span data-ttu-id="e2c84-1411">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e2c84-1411">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e2c84-1412">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="e2c84-1412">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1413">ACS</span></span>

* <span data-ttu-id="e2c84-1414">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="e2c84-1414">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e2c84-1415">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="e2c84-1415">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e2c84-1416">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="e2c84-1416">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e2c84-1417">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1417">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1418">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1418">AppService</span></span>

* <span data-ttu-id="e2c84-1419">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1419">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e2c84-1420">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="e2c84-1420">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e2c84-1421">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1421">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e2c84-1422">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="e2c84-1422">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e2c84-1423">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="e2c84-1423">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e2c84-1424">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1424">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e2c84-1425">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="e2c84-1425">support slot swap with preview</span></span>
* <span data-ttu-id="e2c84-1426">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1426">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e2c84-1427">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1427">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e2c84-1428">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e2c84-1428">CosmosDB</span></span>

* <span data-ttu-id="e2c84-1429">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e2c84-1429">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e2c84-1430">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="e2c84-1430">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e2c84-1431">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="e2c84-1431">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e2c84-1432">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e2c84-1432">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e2c84-1433">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e2c84-1433">Data Lake Analytics</span></span>

* <span data-ttu-id="e2c84-1434">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="e2c84-1434">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e2c84-1435">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1435">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e2c84-1436">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1436">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e2c84-1437">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1437">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e2c84-1438">Table</span><span class="sxs-lookup"><span data-stu-id="e2c84-1438">Table</span></span>
  * <span data-ttu-id="e2c84-1439">Fonction table</span><span class="sxs-lookup"><span data-stu-id="e2c84-1439">Table valued function</span></span>
  * <span data-ttu-id="e2c84-1440">Affichage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1440">View</span></span>
  * <span data-ttu-id="e2c84-1441">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1441">Table Statistics.</span></span> <span data-ttu-id="e2c84-1442">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="e2c84-1442">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e2c84-1443">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1443">Data Lake Store</span></span>

* <span data-ttu-id="e2c84-1444">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="e2c84-1444">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e2c84-1445">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1445">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e2c84-1446">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1446">missed help for access show.</span></span> <span data-ttu-id="e2c84-1447">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1447">adding it.</span></span> <span data-ttu-id="e2c84-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e2c84-1449">Rechercher</span><span class="sxs-lookup"><span data-stu-id="e2c84-1449">Find</span></span>

* <span data-ttu-id="e2c84-1450">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="e2c84-1450">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e2c84-1451">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e2c84-1451">KeyVault</span></span>

* <span data-ttu-id="e2c84-1452">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="e2c84-1452">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e2c84-1453">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="e2c84-1453">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e2c84-1454">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="e2c84-1454">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e2c84-1455">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="e2c84-1455">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e2c84-1456">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1456">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e2c84-1457">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1457">Lab</span></span>

* <span data-ttu-id="e2c84-1458">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1458">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e2c84-1459">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1459">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e2c84-1460">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1460">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e2c84-1461">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1461">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e2c84-1462">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="e2c84-1462">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e2c84-1463">Surveiller</span><span class="sxs-lookup"><span data-stu-id="e2c84-1463">Monitor</span></span>

* <span data-ttu-id="e2c84-1464">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1464">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e2c84-1465">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1465">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e2c84-1466">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1466">Network</span></span>

* <span data-ttu-id="e2c84-1467">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1467">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e2c84-1468">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1468">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e2c84-1469">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="e2c84-1469">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e2c84-1470">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="e2c84-1470">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e2c84-1471">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e2c84-1471">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e2c84-1472">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="e2c84-1472">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e2c84-1473">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="e2c84-1473">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e2c84-1474">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="e2c84-1474">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e2c84-1475">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1475">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e2c84-1476">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="e2c84-1476">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e2c84-1477">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1477">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e2c84-1478">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1478">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e2c84-1479">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1479">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e2c84-1480">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="e2c84-1480">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e2c84-1481">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="e2c84-1481">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e2c84-1482">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="e2c84-1482">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e2c84-1483">Profil</span><span class="sxs-lookup"><span data-stu-id="e2c84-1483">Profile</span></span>

* <span data-ttu-id="e2c84-1484">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1484">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e2c84-1485">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1485">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e2c84-1486">Redis</span><span class="sxs-lookup"><span data-stu-id="e2c84-1486">Redis</span></span>

* <span data-ttu-id="e2c84-1487">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="e2c84-1487">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e2c84-1488">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="e2c84-1488">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e2c84-1489">Ressource</span><span class="sxs-lookup"><span data-stu-id="e2c84-1489">Resource</span></span>

* <span data-ttu-id="e2c84-1490">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1490">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e2c84-1491">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1491">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e2c84-1492">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1492">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e2c84-1493">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1493">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e2c84-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e2c84-1495">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1495">Add docs for az lock update.</span></span> <span data-ttu-id="e2c84-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e2c84-1497">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1497">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e2c84-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e2c84-1499">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1499">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e2c84-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e2c84-1501">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1501">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e2c84-1502">Rôle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1502">Role</span></span>

* <span data-ttu-id="e2c84-1503">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1503">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e2c84-1504">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1504">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e2c84-1505">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1505">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e2c84-1506">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="e2c84-1506">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e2c84-1507">SQL</span><span class="sxs-lookup"><span data-stu-id="e2c84-1507">SQL</span></span>

* <span data-ttu-id="e2c84-1508">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e2c84-1508">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e2c84-1509">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1509">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e2c84-1510">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1510">Storage</span></span>

* <span data-ttu-id="e2c84-1511">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e2c84-1511">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e2c84-1512">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="e2c84-1512">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e2c84-1513">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="e2c84-1513">Add support for large block blob upload</span></span>
* <span data-ttu-id="e2c84-1514">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="e2c84-1514">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1515">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1515">VM</span></span>

* <span data-ttu-id="e2c84-1516">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="e2c84-1516">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e2c84-1517">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1517">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e2c84-1518">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e2c84-1518">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e2c84-1519">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e2c84-1519">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e2c84-1520">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="e2c84-1520">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e2c84-1521">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="e2c84-1521">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e2c84-1522">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1522">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e2c84-1523">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1523">April 3, 2017</span></span>

<span data-ttu-id="e2c84-1524">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e2c84-1524">Version 2.0.2</span></span>

<span data-ttu-id="e2c84-1525">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="e2c84-1525">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="e2c84-1526">Principal</span><span class="sxs-lookup"><span data-stu-id="e2c84-1526">Core</span></span>

* <span data-ttu-id="e2c84-1527">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-1527">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e2c84-1528">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1528">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e2c84-1529">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1529">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e2c84-1530">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1530">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e2c84-1531">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1531">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e2c84-1532">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1532">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e2c84-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e2c84-1534">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="e2c84-1534">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e2c84-1535">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="e2c84-1535">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e2c84-1536">ACS</span><span class="sxs-lookup"><span data-stu-id="e2c84-1536">ACS</span></span>

* <span data-ttu-id="e2c84-1537">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1537">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e2c84-1538">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1538">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e2c84-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e2c84-1540">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1540">Add support for windows clusters.</span></span> <span data-ttu-id="e2c84-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e2c84-1542">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1542">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e2c84-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e2c84-1544">AppService</span><span class="sxs-lookup"><span data-stu-id="e2c84-1544">AppService</span></span>

* <span data-ttu-id="e2c84-1545">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1545">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e2c84-1546">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1546">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e2c84-1547">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1547">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e2c84-1548">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1548">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e2c84-1549">DataLake</span><span class="sxs-lookup"><span data-stu-id="e2c84-1549">DataLake</span></span>

* <span data-ttu-id="e2c84-1550">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e2c84-1550">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e2c84-1551">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e2c84-1551">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e2c84-1552">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e2c84-1552">DocuemntDB</span></span>

* <span data-ttu-id="e2c84-1553">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1553">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e2c84-1554">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="e2c84-1554">VM</span></span>

* <span data-ttu-id="e2c84-1555">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1555">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e2c84-1556">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1556">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e2c84-1557">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1557">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e2c84-1558">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1558">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e2c84-1559">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1559">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e2c84-1560">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1560">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e2c84-1561">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e2c84-1561">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e2c84-1562">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="e2c84-1562">February 27, 2017</span></span>

<span data-ttu-id="e2c84-1563">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e2c84-1563">Version 2.0.0</span></span>

<span data-ttu-id="e2c84-1564">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1564">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e2c84-1565">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1565">Container Service (acs)</span></span>
- <span data-ttu-id="e2c84-1566">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1566">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e2c84-1567">Réseau</span><span class="sxs-lookup"><span data-stu-id="e2c84-1567">Networking</span></span>
- <span data-ttu-id="e2c84-1568">Stockage</span><span class="sxs-lookup"><span data-stu-id="e2c84-1568">Storage</span></span>

<span data-ttu-id="e2c84-1569">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1569">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e2c84-1570">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1570">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e2c84-1571">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1571">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="e2c84-1572">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1572">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e2c84-1573">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="e2c84-1573">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e2c84-1574">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="e2c84-1574">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e2c84-1575">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e2c84-1575">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e2c84-1576">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e2c84-1576">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e2c84-1577">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e2c84-1577">Provide feedback from the command line with the `az feedback` command</span></span>

