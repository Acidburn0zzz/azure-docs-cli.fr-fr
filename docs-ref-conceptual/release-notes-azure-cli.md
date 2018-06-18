---
title: Notes de publication d’Azure CLI 2.0
description: En savoir plus sur les dernières mises à jour d’Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 72e667d74ff8d55f26ecbf3b3c8845c9c03b56be
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512901"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="a8ca3-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a8ca3-104">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-104">June 13, 2018</span></span>

<span data-ttu-id="a8ca3-105">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a8ca3-105">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a8ca3-106">AKS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-106">AKS</span></span>

* <span data-ttu-id="a8ca3-107">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-107">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a8ca3-108">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="a8ca3-108">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="a8ca3-109">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-109">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a8ca3-110">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-110">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a8ca3-111">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-111">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-112">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-112">AppService</span></span>

* <span data-ttu-id="a8ca3-113">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="a8ca3-113">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a8ca3-114">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-114">June 5, 2018</span></span>

<span data-ttu-id="a8ca3-115">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a8ca3-115">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-116">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-116">Interactive</span></span>

* <span data-ttu-id="a8ca3-117">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-117">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a8ca3-118">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-118">June 5, 2018</span></span>

<span data-ttu-id="a8ca3-119">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a8ca3-119">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-120">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-120">Core</span></span>

* <span data-ttu-id="a8ca3-121">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="a8ca3-121">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a8ca3-122">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-122">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-123">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-123">ACR</span></span>

* <span data-ttu-id="a8ca3-124">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="a8ca3-124">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a8ca3-125">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-125">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a8ca3-126">AKS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-126">AKS</span></span>

* <span data-ttu-id="a8ca3-127">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-127">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-128">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-128">Batch</span></span>

* <span data-ttu-id="a8ca3-129">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a8ca3-129">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-130">IOT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-130">IOT</span></span>

* <span data-ttu-id="a8ca3-131">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="a8ca3-131">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-132">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-132">Network</span></span>

* <span data-ttu-id="a8ca3-133">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="a8ca3-133">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a8ca3-134">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a8ca3-134">Policy Insights</span></span>

* <span data-ttu-id="a8ca3-135">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-135">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a8ca3-136">ARM</span><span class="sxs-lookup"><span data-stu-id="a8ca3-136">ARM</span></span>

* <span data-ttu-id="a8ca3-137">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-137">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-138">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-138">SQL</span></span>

* <span data-ttu-id="a8ca3-139">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-139">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a8ca3-140">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-140">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a8ca3-141">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-141">Storage</span></span>

* <span data-ttu-id="a8ca3-142">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="a8ca3-142">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-143">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-143">VM</span></span>

* <span data-ttu-id="a8ca3-144">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-144">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a8ca3-145">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-145">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a8ca3-146">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-146">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a8ca3-147">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-147">May 22, 2018</span></span>

<span data-ttu-id="a8ca3-148">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a8ca3-148">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-149">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-149">Core</span></span>

* <span data-ttu-id="a8ca3-150">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="a8ca3-150">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-151">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-151">ACS</span></span>

* <span data-ttu-id="a8ca3-152">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-152">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a8ca3-153">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="a8ca3-153">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-154">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-154">AppService</span></span>

* <span data-ttu-id="a8ca3-155">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-155">Improved generic update commands</span></span>
* <span data-ttu-id="a8ca3-156">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-156">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-157">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-157">Container</span></span>

* <span data-ttu-id="a8ca3-158">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="a8ca3-158">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a8ca3-159">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-159">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-160">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-160">Extension</span></span>

* <span data-ttu-id="a8ca3-161">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-161">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-162">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-162">Interactive</span></span>

* <span data-ttu-id="a8ca3-163">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="a8ca3-163">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a8ca3-164">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="a8ca3-164">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-165">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-165">KeyVault</span></span>

* <span data-ttu-id="a8ca3-166">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a8ca3-166">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-167">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-167">Network</span></span>

* <span data-ttu-id="a8ca3-168">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-168">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a8ca3-169">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-169">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-170">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-170">SQL</span></span>

* <span data-ttu-id="a8ca3-171">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-171">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a8ca3-172">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-172">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a8ca3-173">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-173">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="a8ca3-174">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a8ca3-174">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a8ca3-175">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-175">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a8ca3-176">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-176">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a8ca3-177">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-177">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a8ca3-178">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-178">`edition`.</span></span> <span data-ttu-id="a8ca3-179">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-179">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a8ca3-180">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-180">`elasticPoolName`.</span></span> <span data-ttu-id="a8ca3-181">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-181">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a8ca3-182">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-182">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a8ca3-183">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-183">`edition`.</span></span> <span data-ttu-id="a8ca3-184">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-184">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a8ca3-185">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-185">`dtu`.</span></span> <span data-ttu-id="a8ca3-186">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-186">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a8ca3-187">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-187">`databaseDtuMin`.</span></span> <span data-ttu-id="a8ca3-188">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-188">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a8ca3-189">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-189">`databaseDtuMax`.</span></span> <span data-ttu-id="a8ca3-190">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-190">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a8ca3-191">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-191">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a8ca3-192">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-192">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-193">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-193">Storage</span></span>

* <span data-ttu-id="a8ca3-194">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-194">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a8ca3-195">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-195">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-196">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-196">VM</span></span>

* <span data-ttu-id="a8ca3-197">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-197">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a8ca3-198">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-198">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a8ca3-199">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-199">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a8ca3-200">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-200">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a8ca3-201">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-201">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a8ca3-202">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-202">May 7, 2018</span></span>

<span data-ttu-id="a8ca3-203">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a8ca3-203">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-204">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-204">Core</span></span>

* <span data-ttu-id="a8ca3-205">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="a8ca3-205">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a8ca3-206">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="a8ca3-206">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a8ca3-207">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-207">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a8ca3-208">#5591</span><span class="sxs-lookup"><span data-stu-id="a8ca3-208">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a8ca3-209">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-209">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a8ca3-210">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="a8ca3-210">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a8ca3-211">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-211">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a8ca3-212">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-212">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a8ca3-213">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-213">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-214">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-214">ACR</span></span>

* <span data-ttu-id="a8ca3-215">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-215">Added ACR Build commands</span></span>
* <span data-ttu-id="a8ca3-216">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="a8ca3-216">Improved resource not found error messages</span></span>
* <span data-ttu-id="a8ca3-217">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-217">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a8ca3-218">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-218">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a8ca3-219">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="a8ca3-219">Improved repository commands error messages</span></span>
* <span data-ttu-id="a8ca3-220">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-220">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-221">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-221">ACS</span></span>

* <span data-ttu-id="a8ca3-222">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="a8ca3-222">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a8ca3-223">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a8ca3-223">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a8ca3-224">AMS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-224">AMS</span></span>

* <span data-ttu-id="a8ca3-225">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="a8ca3-225">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-226">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-226">Appservice</span></span>

* <span data-ttu-id="a8ca3-227">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="a8ca3-227">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a8ca3-228">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-228">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a8ca3-229">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-229">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a8ca3-230">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-230">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a8ca3-231">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-231">Batch AI</span></span>

* <span data-ttu-id="a8ca3-232">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="a8ca3-232">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a8ca3-233">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a8ca3-233">Cognitive Services</span></span>

* <span data-ttu-id="a8ca3-234">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-234">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a8ca3-235">Consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-235">Consumption</span></span>

* <span data-ttu-id="a8ca3-236">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="a8ca3-236">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-237">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-237">Container</span></span>

* <span data-ttu-id="a8ca3-238">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="a8ca3-238">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a8ca3-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-239">Cosmos DB</span></span>

* <span data-ttu-id="a8ca3-240">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-240">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a8ca3-241">DMS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-241">DMS</span></span>

* <span data-ttu-id="a8ca3-242">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="a8ca3-242">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-243">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-243">Extension</span></span>

* <span data-ttu-id="a8ca3-244">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-244">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-245">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-245">Interactive</span></span>

* <span data-ttu-id="a8ca3-246">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="a8ca3-246">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a8ca3-247">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="a8ca3-247">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a8ca3-248">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="a8ca3-248">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a8ca3-249">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-249">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a8ca3-250">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-250">Lab</span></span>

* <span data-ttu-id="a8ca3-251">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="a8ca3-251">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-252">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-252">Network</span></span>

* <span data-ttu-id="a8ca3-253">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-253">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a8ca3-254">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-254">Profile</span></span>

* <span data-ttu-id="a8ca3-255">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-255">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a8ca3-256">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-256">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a8ca3-257">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-257">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a8ca3-258">Redis</span><span class="sxs-lookup"><span data-stu-id="a8ca3-258">Redis</span></span>

* <span data-ttu-id="a8ca3-259">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-259">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a8ca3-260">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-260">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a8ca3-261">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-261">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a8ca3-262">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-262">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a8ca3-263">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-263">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-264">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-264">Role</span></span>

* <span data-ttu-id="a8ca3-265">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a8ca3-265">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-266">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-266">Storage</span></span>

* <span data-ttu-id="a8ca3-267">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-267">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a8ca3-268">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="a8ca3-268">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a8ca3-269">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-269">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a8ca3-270">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-270">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a8ca3-271">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-271">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-272">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-272">VM</span></span>

* <span data-ttu-id="a8ca3-273">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-273">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a8ca3-274">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-274">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a8ca3-275">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-275">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a8ca3-276">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-276">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a8ca3-277">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-277">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a8ca3-278">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="a8ca3-278">Added write accelerator support</span></span> 
* <span data-ttu-id="a8ca3-279">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-279">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a8ca3-280">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-280">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a8ca3-281">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="a8ca3-281">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a8ca3-282">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-282">April 10, 2018</span></span>

<span data-ttu-id="a8ca3-283">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a8ca3-283">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-284">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-284">ACR</span></span>

* <span data-ttu-id="a8ca3-285">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="a8ca3-285">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-286">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-286">ACS</span></span>

* <span data-ttu-id="a8ca3-287">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="a8ca3-287">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-288">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-288">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a8ca3-290">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="a8ca3-290">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a8ca3-291">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-291">BatchAI</span></span>

* <span data-ttu-id="a8ca3-292">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="a8ca3-292">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="a8ca3-293">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-293">Job level mounting</span></span>
 - <span data-ttu-id="a8ca3-294">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="a8ca3-294">Environment variables with secret values</span></span>
 - <span data-ttu-id="a8ca3-295">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="a8ca3-295">Performance counters settings</span></span>
 - <span data-ttu-id="a8ca3-296">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-296">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="a8ca3-297">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="a8ca3-297">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="a8ca3-298">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="a8ca3-298">Usage and limits reporting</span></span>
 - <span data-ttu-id="a8ca3-299">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-299">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="a8ca3-300">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-300">Support for custom images</span></span>
 - <span data-ttu-id="a8ca3-301">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-301">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a8ca3-302">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-302">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a8ca3-303">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-303">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a8ca3-304">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="a8ca3-304">National clouds are supported</span></span>
* <span data-ttu-id="a8ca3-305">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="a8ca3-305">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a8ca3-306">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-306">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a8ca3-307">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-307">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a8ca3-308">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-308">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a8ca3-309">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-309">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a8ca3-310">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-310">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a8ca3-311">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-311">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a8ca3-312">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-312">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a8ca3-313">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="a8ca3-313">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a8ca3-314">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-314">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a8ca3-315">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-315">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a8ca3-316">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-316">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a8ca3-317">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-317">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a8ca3-318">Facturation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-318">Billing</span></span>

* <span data-ttu-id="a8ca3-319">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="a8ca3-319">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a8ca3-320">Consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-320">Consumption</span></span>

* <span data-ttu-id="a8ca3-321">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-321">Added `marketplace` commands</span></span>
* <span data-ttu-id="a8ca3-322">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-322">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a8ca3-323">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-323">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a8ca3-324">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-324">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a8ca3-325">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-325">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a8ca3-326">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-326">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-327">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-327">Container</span></span>

* <span data-ttu-id="a8ca3-328">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-328">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a8ca3-329">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="a8ca3-329">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-330">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-330">Extension</span></span>

* <span data-ttu-id="a8ca3-331">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-331">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-332">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-332">Interactive</span></span>

* <span data-ttu-id="a8ca3-333">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="a8ca3-333">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a8ca3-334">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-334">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a8ca3-335">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-335">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-336">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-336">Network</span></span>

* <span data-ttu-id="a8ca3-337">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="a8ca3-337">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a8ca3-338">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-338">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a8ca3-339">#4910</span><span class="sxs-lookup"><span data-stu-id="a8ca3-339">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a8ca3-340">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-340">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="a8ca3-341">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-341">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a8ca3-342">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-342">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a8ca3-343">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-343">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a8ca3-344">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-344">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-345">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-345">Profile</span></span>

* <span data-ttu-id="a8ca3-346">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-346">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a8ca3-347">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-347">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a8ca3-348">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-348">RDBMS</span></span>

* <span data-ttu-id="a8ca3-349">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-349">Added `georestore` command</span></span>
* <span data-ttu-id="a8ca3-350">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-350">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-351">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-351">Resource</span></span>

* <span data-ttu-id="a8ca3-352">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-352">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a8ca3-353">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-353">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-354">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-354">SQL</span></span>

* <span data-ttu-id="a8ca3-355">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-355">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-356">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-356">Storage</span></span>

* <span data-ttu-id="a8ca3-357">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-357">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-358">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-358">VM</span></span>

* <span data-ttu-id="a8ca3-359">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-359">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a8ca3-360">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-360">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a8ca3-362">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-362">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a8ca3-363">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-363">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a8ca3-364">#5718</span><span class="sxs-lookup"><span data-stu-id="a8ca3-364">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a8ca3-365">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="a8ca3-365">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a8ca3-366">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-366">March 27, 2018</span></span>

<span data-ttu-id="a8ca3-367">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a8ca3-367">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-368">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-368">Core</span></span>

* <span data-ttu-id="a8ca3-369">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="a8ca3-369">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-370">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-370">ACS</span></span>

* <span data-ttu-id="a8ca3-371">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a8ca3-371">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-372">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-372">Appservice</span></span>

* <span data-ttu-id="a8ca3-373">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-373">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a8ca3-374">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-374">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a8ca3-375">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a8ca3-375">Backup</span></span>

* <span data-ttu-id="a8ca3-376">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-376">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a8ca3-377">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-377">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a8ca3-378">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-378">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a8ca3-379">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-379">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-380">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-380">Container</span></span>

* <span data-ttu-id="a8ca3-381">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-381">Added `container exec` command.</span></span> <span data-ttu-id="a8ca3-382">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-382">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a8ca3-383">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-383">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-384">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-384">Extension</span></span>

* <span data-ttu-id="a8ca3-385">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="a8ca3-385">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a8ca3-386">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-386">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a8ca3-387">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-387">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-388">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-388">Interactive</span></span>

* <span data-ttu-id="a8ca3-389">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-389">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a8ca3-390">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-390">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a8ca3-391">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="a8ca3-391">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a8ca3-392">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="a8ca3-392">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a8ca3-393">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-393">Lab</span></span>

* <span data-ttu-id="a8ca3-394">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-394">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-395">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-395">Monitor</span></span>

* <span data-ttu-id="a8ca3-396">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-396">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a8ca3-397">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="a8ca3-397">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a8ca3-398">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-398">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-399">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-399">Network</span></span>

* <span data-ttu-id="a8ca3-400">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="a8ca3-400">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-401">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-401">Profile</span></span>

* <span data-ttu-id="a8ca3-402">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-402">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a8ca3-403">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-403">RDBMS</span></span>

* <span data-ttu-id="a8ca3-404">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a8ca3-404">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-405">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-405">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a8ca3-407">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-407">Role</span></span>

* <span data-ttu-id="a8ca3-408">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-408">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a8ca3-409">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="a8ca3-409">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a8ca3-410">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-410">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a8ca3-411">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-411">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a8ca3-412">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-412">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-413">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-413">Storage</span></span>

* <span data-ttu-id="a8ca3-414">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="a8ca3-414">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a8ca3-415">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="a8ca3-415">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-416">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-416">VM</span></span>

* <span data-ttu-id="a8ca3-417">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="a8ca3-417">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a8ca3-418">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-418">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a8ca3-419">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-419">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a8ca3-420">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-420">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a8ca3-421">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-421">March 13, 2018</span></span>

<span data-ttu-id="a8ca3-422">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a8ca3-422">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-423">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-423">ACR</span></span>

* <span data-ttu-id="a8ca3-424">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-424">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a8ca3-425">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-425">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a8ca3-426">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="a8ca3-426">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-427">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-427">ACS</span></span>

* <span data-ttu-id="a8ca3-428">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="a8ca3-428">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a8ca3-429">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="a8ca3-429">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a8ca3-430">Advisor</span><span class="sxs-lookup"><span data-stu-id="a8ca3-430">Advisor</span></span>

* <span data-ttu-id="a8ca3-431">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-431">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a8ca3-432">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-432">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a8ca3-433">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-433">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="a8ca3-434">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-434">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a8ca3-435">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-435">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-436">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-436">Appservice</span></span>

* <span data-ttu-id="a8ca3-437">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a8ca3-437">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a8ca3-438">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-438">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a8ca3-439">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-439">Eventhubs</span></span>

* <span data-ttu-id="a8ca3-440">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-440">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-441">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-441">Extension</span></span>

* <span data-ttu-id="a8ca3-442">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-442">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-443">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-443">Interactive</span></span>

* <span data-ttu-id="a8ca3-444">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-444">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a8ca3-445">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-445">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a8ca3-446">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="a8ca3-446">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a8ca3-447">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="a8ca3-447">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-448">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-448">Monitor</span></span>

* <span data-ttu-id="a8ca3-449">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-449">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a8ca3-450">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-450">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a8ca3-451">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-451">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a8ca3-452">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-452">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-453">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-453">Network</span></span>

* <span data-ttu-id="a8ca3-454">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-454">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a8ca3-455">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-455">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a8ca3-456">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-456">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a8ca3-457">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-457">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-458">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-458">Profile</span></span>

* <span data-ttu-id="a8ca3-459">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-459">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a8ca3-460">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-460">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a8ca3-461">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-461">RDBMS</span></span>

* <span data-ttu-id="a8ca3-462">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="a8ca3-462">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a8ca3-463">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a8ca3-463">Service Bus</span></span>

* <span data-ttu-id="a8ca3-464">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-464">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-465">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-465">Storage</span></span>

* <span data-ttu-id="a8ca3-466">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="a8ca3-466">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a8ca3-467">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="a8ca3-467">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-468">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-468">VM</span></span>

* <span data-ttu-id="a8ca3-469">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="a8ca3-469">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a8ca3-470">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-470">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a8ca3-471">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-471">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a8ca3-472">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="a8ca3-472">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a8ca3-473">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-473">February 27, 2018</span></span>

<span data-ttu-id="a8ca3-474">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a8ca3-474">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-475">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-475">Core</span></span>

* <span data-ttu-id="a8ca3-476">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="a8ca3-476">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a8ca3-477">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-477">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a8ca3-478">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-478">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-479">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-479">ACS</span></span>

* <span data-ttu-id="a8ca3-480">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-480">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a8ca3-481">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-481">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a8ca3-482">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-482">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a8ca3-483">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-483">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-484">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-484">Appservice</span></span>

* <span data-ttu-id="a8ca3-485">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-485">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a8ca3-486">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="a8ca3-486">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a8ca3-487">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a8ca3-487">Cognitive Services</span></span>

* <span data-ttu-id="a8ca3-488">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a8ca3-488">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a8ca3-489">Consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-489">Consumption</span></span>

* <span data-ttu-id="a8ca3-490">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="a8ca3-490">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a8ca3-491">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-491">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-492">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-492">Container</span></span>

* <span data-ttu-id="a8ca3-493">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-493">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-494">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-494">Network</span></span>

* <span data-ttu-id="a8ca3-495">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-495">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-496">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-496">Resource</span></span>

* <span data-ttu-id="a8ca3-497">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="a8ca3-497">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-498">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-498">Role</span></span>

* <span data-ttu-id="a8ca3-499">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="a8ca3-499">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-500">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-500">SQL</span></span>

* <span data-ttu-id="a8ca3-501">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="a8ca3-501">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-502">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-502">Storage</span></span>

* <span data-ttu-id="a8ca3-503">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-503">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-504">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-504">VM</span></span>

* <span data-ttu-id="a8ca3-505">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="a8ca3-505">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a8ca3-506">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-506">February 13, 2018</span></span>

<span data-ttu-id="a8ca3-507">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a8ca3-507">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-508">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-508">Core</span></span>

* <span data-ttu-id="a8ca3-509">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-509">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-510">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-510">ACS</span></span>

* <span data-ttu-id="a8ca3-511">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="a8ca3-511">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a8ca3-512">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-512">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a8ca3-513">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-513">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a8ca3-514">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-514">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a8ca3-515">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-515">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a8ca3-516">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-516">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a8ca3-517">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-517">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a8ca3-518">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-518">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-519">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-519">Appservice</span></span>

* <span data-ttu-id="a8ca3-520">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="a8ca3-520">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a8ca3-521">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-521">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a8ca3-522">CDN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-522">CDN</span></span>

* <span data-ttu-id="a8ca3-523">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-523">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-524">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-524">Container</span></span>

* <span data-ttu-id="a8ca3-525">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="a8ca3-525">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a8ca3-526">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-526">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a8ca3-527">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-527">CosmosDB</span></span>

* <span data-ttu-id="a8ca3-528">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a8ca3-528">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-529">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-529">Extension</span></span>

* <span data-ttu-id="a8ca3-530">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-530">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a8ca3-531">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-531">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a8ca3-532">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a8ca3-532">Feedback</span></span>

* <span data-ttu-id="a8ca3-533">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-533">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-534">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-534">Interactive</span></span>

* <span data-ttu-id="a8ca3-535">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a8ca3-535">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a8ca3-536">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="a8ca3-536">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-537">IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-537">IoT</span></span>

* <span data-ttu-id="a8ca3-538">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a8ca3-538">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a8ca3-539">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a8ca3-539">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a8ca3-540">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-540">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a8ca3-541">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-541">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-542">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-542">Monitor</span></span>

* <span data-ttu-id="a8ca3-543">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-543">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-544">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-544">Network</span></span>

* <span data-ttu-id="a8ca3-545">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-545">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a8ca3-546">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-546">Profile</span></span>

* <span data-ttu-id="a8ca3-547">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-547">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-548">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-548">Resource</span></span>

* <span data-ttu-id="a8ca3-549">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-549">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-550">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-550">Role</span></span>

* <span data-ttu-id="a8ca3-551">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-551">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-552">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-552">SQL</span></span>

* <span data-ttu-id="a8ca3-553">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-553">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a8ca3-554">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-554">Added `sql db rename`</span></span>
* <span data-ttu-id="a8ca3-555">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="a8ca3-555">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-556">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-556">Storage</span></span>

* <span data-ttu-id="a8ca3-557">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="a8ca3-557">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-558">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-558">VM</span></span>

* <span data-ttu-id="a8ca3-559">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-559">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a8ca3-560">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-560">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a8ca3-561">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-561">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a8ca3-562">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-562">January 31, 2018</span></span>

<span data-ttu-id="a8ca3-563">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a8ca3-563">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-564">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-564">Core</span></span>

* <span data-ttu-id="a8ca3-565">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-565">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a8ca3-566">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="a8ca3-566">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a8ca3-567">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-567">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a8ca3-568">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="a8ca3-568">Use `--verbose` to see</span></span>
* <span data-ttu-id="a8ca3-569">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="a8ca3-569">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-570">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-570">ACS</span></span>

* <span data-ttu-id="a8ca3-571">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-571">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a8ca3-572">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-572">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-573">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-573">Appservice</span></span>

* <span data-ttu-id="a8ca3-574">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-574">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a8ca3-575">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="a8ca3-575">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a8ca3-576">CDN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-576">CDN</span></span>

* <span data-ttu-id="a8ca3-577">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-577">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a8ca3-578">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-578">CosmosDB</span></span>

* <span data-ttu-id="a8ca3-579">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-579">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-580">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-580">Interactive</span></span>

* <span data-ttu-id="a8ca3-581">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="a8ca3-581">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-582">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-582">Network</span></span>

* <span data-ttu-id="a8ca3-583">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-583">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a8ca3-584">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-584">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a8ca3-585">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-585">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a8ca3-586">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-586">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a8ca3-587">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-587">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a8ca3-588">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-588">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a8ca3-589">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-589">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a8ca3-590">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-590">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a8ca3-591">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-591">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="a8ca3-592">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-592">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-593">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-593">Profile</span></span>

* <span data-ttu-id="a8ca3-594">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a8ca3-594">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-595">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-595">Resource</span></span>

* <span data-ttu-id="a8ca3-596">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="a8ca3-596">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-597">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-597">Storage</span></span>

* <span data-ttu-id="a8ca3-598">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="a8ca3-598">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a8ca3-599">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-599">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a8ca3-600">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-600">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="a8ca3-601">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-601">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a8ca3-602">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="a8ca3-602">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-603">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-603">VM</span></span>

* <span data-ttu-id="a8ca3-604">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="a8ca3-604">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a8ca3-605">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-605">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a8ca3-606">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="a8ca3-606">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a8ca3-607">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-607">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a8ca3-608">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a8ca3-608">January 17, 2018</span></span>

<span data-ttu-id="a8ca3-609">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a8ca3-609">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-610">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-610">ACR</span></span>

* <span data-ttu-id="a8ca3-611">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="a8ca3-611">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a8ca3-612">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="a8ca3-612">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-613">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-613">ACS</span></span>

* <span data-ttu-id="a8ca3-614">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-614">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a8ca3-615">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-615">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-616">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-616">Appservice</span></span>

* <span data-ttu-id="a8ca3-617">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="a8ca3-617">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a8ca3-618">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-618">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a8ca3-619">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-619">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a8ca3-620">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a8ca3-620">Backup</span></span>

* <span data-ttu-id="a8ca3-621">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="a8ca3-621">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a8ca3-622">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-622">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a8ca3-623">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="a8ca3-623">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a8ca3-624">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="a8ca3-624">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a8ca3-625">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-625">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-626">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-626">Batch</span></span>

* <span data-ttu-id="a8ca3-627">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="a8ca3-627">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a8ca3-628">Cloud</span><span class="sxs-lookup"><span data-stu-id="a8ca3-628">Cloud</span></span>

* <span data-ttu-id="a8ca3-629">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="a8ca3-629">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a8ca3-630">Consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-630">Consumption</span></span>

* <span data-ttu-id="a8ca3-631">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-631">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a8ca3-632">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a8ca3-632">Event Grid</span></span>

* <span data-ttu-id="a8ca3-633">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-633">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a8ca3-634">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-634">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a8ca3-635">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-635">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a8ca3-636">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="a8ca3-636">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a8ca3-637">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-637">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a8ca3-638">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-638">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a8ca3-639">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-639">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a8ca3-640">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-640">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-641">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-641">Interactive</span></span>

* <span data-ttu-id="a8ca3-642">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="a8ca3-642">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a8ca3-643">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-643">Fixed errors on startup</span></span>
* <span data-ttu-id="a8ca3-644">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-644">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-645">IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-645">IoT</span></span>

* <span data-ttu-id="a8ca3-646">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="a8ca3-646">Added support for device provisioning service</span></span>
* <span data-ttu-id="a8ca3-647">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-647">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a8ca3-648">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-648">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-649">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-649">Monitor</span></span>

* <span data-ttu-id="a8ca3-650">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-650">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a8ca3-651">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-651">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a8ca3-652">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="a8ca3-652">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-653">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-653">Network</span></span>

* <span data-ttu-id="a8ca3-654">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-654">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a8ca3-655">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-655">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-656">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-656">Profile</span></span>

* <span data-ttu-id="a8ca3-657">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-657">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-658">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-658">Role</span></span>

* <span data-ttu-id="a8ca3-659">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-659">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a8ca3-660">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a8ca3-660">Service Fabric</span></span>

* <span data-ttu-id="a8ca3-661">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="a8ca3-661">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a8ca3-662">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-662">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-663">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-663">VM</span></span>

* <span data-ttu-id="a8ca3-664">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-664">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a8ca3-665">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-665">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a8ca3-666">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-666">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a8ca3-667">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-667">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a8ca3-668">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="a8ca3-668">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a8ca3-669">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-669">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a8ca3-670">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-670">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a8ca3-671">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-671">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a8ca3-672">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-672">December 19, 2017</span></span>

<span data-ttu-id="a8ca3-673">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a8ca3-673">Version 2.0.23</span></span>

* <span data-ttu-id="a8ca3-674">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-674">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-675">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-675">Container</span></span>

* <span data-ttu-id="a8ca3-676">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-676">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-677">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-677">Network</span></span>

* <span data-ttu-id="a8ca3-678">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-678">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a8ca3-679">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-679">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-680">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-680">Storage</span></span>

* <span data-ttu-id="a8ca3-681">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="a8ca3-681">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-682">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-682">VM</span></span>

* <span data-ttu-id="a8ca3-683">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-683">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a8ca3-684">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-684">December 5, 2017</span></span>

<span data-ttu-id="a8ca3-685">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a8ca3-685">Version 2.0.22</span></span>

* <span data-ttu-id="a8ca3-686">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-686">Removed `az component` commands.</span></span> <span data-ttu-id="a8ca3-687">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="a8ca3-687">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-688">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-688">Core</span></span>
* <span data-ttu-id="a8ca3-689">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="a8ca3-689">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a8ca3-690">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-690">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-691">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-691">ACS</span></span>

* <span data-ttu-id="a8ca3-692">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-692">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a8ca3-693">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-693">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a8ca3-694">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="a8ca3-694">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a8ca3-695">Advisor</span><span class="sxs-lookup"><span data-stu-id="a8ca3-695">Advisor</span></span>

* <span data-ttu-id="a8ca3-696">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-696">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-697">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-697">Appservice</span></span>

* <span data-ttu-id="a8ca3-698">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-698">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a8ca3-699">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-699">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a8ca3-700">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-700">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a8ca3-701">Consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-701">Consumption</span></span>

* <span data-ttu-id="a8ca3-702">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="a8ca3-702">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-703">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-703">Container</span></span>

* <span data-ttu-id="a8ca3-704">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-704">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-705">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-705">Monitor</span></span>

* <span data-ttu-id="a8ca3-706">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="a8ca3-706">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-707">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-707">Resource</span></span>

* <span data-ttu-id="a8ca3-708">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-708">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-709">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-709">Role</span></span>

* <span data-ttu-id="a8ca3-710">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-710">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a8ca3-711">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-711">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a8ca3-712">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-712">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-713">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-713">SQL</span></span>

* <span data-ttu-id="a8ca3-714">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-714">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a8ca3-715">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-715">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-716">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-716">VM</span></span>

* <span data-ttu-id="a8ca3-717">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-717">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a8ca3-718">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-718">November 14, 2017</span></span>

<span data-ttu-id="a8ca3-719">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a8ca3-719">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-720">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-720">ACR</span></span>

* <span data-ttu-id="a8ca3-721">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="a8ca3-721">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a8ca3-722">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-722">ACS</span></span>

* <span data-ttu-id="a8ca3-723">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-723">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a8ca3-724">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-724">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a8ca3-725">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-725">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a8ca3-726">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a8ca3-726">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a8ca3-727">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a8ca3-727">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-728">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-728">Appservice</span></span>

* <span data-ttu-id="a8ca3-729">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="a8ca3-729">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a8ca3-730">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-730">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a8ca3-731">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-731">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a8ca3-732">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-732">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a8ca3-733">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="a8ca3-733">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a8ca3-734">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-734">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-735">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-735">Batch</span></span>

* <span data-ttu-id="a8ca3-736">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-736">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a8ca3-737">Batchai</span><span class="sxs-lookup"><span data-stu-id="a8ca3-737">Batchai</span></span>

* <span data-ttu-id="a8ca3-738">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-738">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a8ca3-739">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-739">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a8ca3-740">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-740">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a8ca3-741">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-741">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a8ca3-742">Cloud</span><span class="sxs-lookup"><span data-stu-id="a8ca3-742">Cloud</span></span>

* <span data-ttu-id="a8ca3-743">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="a8ca3-743">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-744">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-744">Container</span></span>

* <span data-ttu-id="a8ca3-745">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="a8ca3-745">Added support to open multiple ports</span></span>
* <span data-ttu-id="a8ca3-746">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-746">Added container group restart policy</span></span>
* <span data-ttu-id="a8ca3-747">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="a8ca3-747">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a8ca3-748">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="a8ca3-748">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a8ca3-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a8ca3-749">Data Lake Analytics</span></span>

* <span data-ttu-id="a8ca3-750">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a8ca3-750">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a8ca3-751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-751">Data Lake Store</span></span>

* <span data-ttu-id="a8ca3-752">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a8ca3-752">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-753">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-753">Extension</span></span>

* <span data-ttu-id="a8ca3-754">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8ca3-754">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a8ca3-755">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="a8ca3-755">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-756">IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-756">IoT</span></span>

* <span data-ttu-id="a8ca3-757">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-757">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-758">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-758">Monitor</span></span>

* <span data-ttu-id="a8ca3-759">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-759">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-760">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-760">Network</span></span>

* <span data-ttu-id="a8ca3-761">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="a8ca3-761">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a8ca3-762">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-762">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a8ca3-763">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a8ca3-763">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a8ca3-764">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-764">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a8ca3-765">Réservations</span><span class="sxs-lookup"><span data-stu-id="a8ca3-765">Reservations</span></span>

* <span data-ttu-id="a8ca3-766">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-766">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-767">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-767">Resource</span></span>

* <span data-ttu-id="a8ca3-768">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a8ca3-768">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-769">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-769">SQL</span></span>

* <span data-ttu-id="a8ca3-770">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-770">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-771">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-771">Storage</span></span>

* <span data-ttu-id="a8ca3-772">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-772">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a8ca3-773">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="a8ca3-773">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a8ca3-774">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-774">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a8ca3-775">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-775">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a8ca3-776">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-776">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a8ca3-777">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-777">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a8ca3-778">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-778">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-779">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-779">VM</span></span>

* <span data-ttu-id="a8ca3-780">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-780">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a8ca3-781">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-781">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a8ca3-782">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="a8ca3-782">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a8ca3-783">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-783">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a8ca3-784">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-784">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a8ca3-785">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-785">October 24, 2017</span></span>

<span data-ttu-id="a8ca3-786">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a8ca3-786">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-787">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-787">Core</span></span>

* <span data-ttu-id="a8ca3-788">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-788">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-789">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-789">ACR</span></span>

* <span data-ttu-id="a8ca3-790">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-790">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a8ca3-791">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-791">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a8ca3-792">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="a8ca3-792">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-793">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-793">ACS</span></span>

* <span data-ttu-id="a8ca3-794">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-794">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a8ca3-795">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-795">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-796">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-796">Appservice</span></span>

* <span data-ttu-id="a8ca3-797">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="a8ca3-797">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a8ca3-798">Composant</span><span class="sxs-lookup"><span data-stu-id="a8ca3-798">Component</span></span>

* <span data-ttu-id="a8ca3-799">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-799">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-800">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-800">Monitor</span></span>

* <span data-ttu-id="a8ca3-801">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-801">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-802">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-802">Resource</span></span>

* <span data-ttu-id="a8ca3-803">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-803">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a8ca3-804">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-804">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-805">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-805">VM</span></span>

* <span data-ttu-id="a8ca3-806">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-806">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a8ca3-807">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-807">October 9, 2017</span></span>

<span data-ttu-id="a8ca3-808">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a8ca3-808">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-809">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-809">Core</span></span>

* <span data-ttu-id="a8ca3-810">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a8ca3-810">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-811">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-811">Appservice</span></span>

* <span data-ttu-id="a8ca3-812">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-812">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-813">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-813">Batch</span></span>

* <span data-ttu-id="a8ca3-814">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-814">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a8ca3-815">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="a8ca3-815">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a8ca3-816">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-816">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a8ca3-817">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="a8ca3-817">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a8ca3-818">Batchai</span><span class="sxs-lookup"><span data-stu-id="a8ca3-818">Batchai</span></span>

* <span data-ttu-id="a8ca3-819">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="a8ca3-819">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-820">Keyvault</span></span>

* <span data-ttu-id="a8ca3-821">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-821">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a8ca3-822">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-822">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a8ca3-823">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-823">Network</span></span>

* <span data-ttu-id="a8ca3-824">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="a8ca3-824">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a8ca3-825">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-825">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-826">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-826">Resource</span></span>

* <span data-ttu-id="a8ca3-827">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-827">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a8ca3-828">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-828">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a8ca3-829">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-829">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a8ca3-830">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a8ca3-830">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-831">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-831">Sql</span></span>

* <span data-ttu-id="a8ca3-832">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="a8ca3-832">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a8ca3-833">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-833">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a8ca3-834">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="a8ca3-834">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-835">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-835">Storage</span></span>

* <span data-ttu-id="a8ca3-836">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="a8ca3-836">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-837">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-837">Vm</span></span>

* <span data-ttu-id="a8ca3-838">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-838">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a8ca3-839">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-839">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a8ca3-840">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-840">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a8ca3-841">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-841">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a8ca3-842">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-842">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a8ca3-843">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-843">September 22, 2017</span></span>

<span data-ttu-id="a8ca3-844">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a8ca3-844">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-845">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-845">Resource</span></span>

* <span data-ttu-id="a8ca3-846">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-846">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a8ca3-847">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-847">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a8ca3-848">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-848">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a8ca3-849">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-849">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-850">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-850">Network</span></span>

* <span data-ttu-id="a8ca3-851">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-851">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a8ca3-852">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-852">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a8ca3-853">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-853">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a8ca3-854">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-854">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a8ca3-855">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-855">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a8ca3-856">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-856">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a8ca3-857">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-857">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-858">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-858">Storage</span></span>

* <span data-ttu-id="a8ca3-859">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-859">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a8ca3-860">Événement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-860">Eventgrid</span></span>

* <span data-ttu-id="a8ca3-861">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-861">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-862">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-862">SQL</span></span>

* <span data-ttu-id="a8ca3-863">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-863">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a8ca3-864">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-864">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a8ca3-865">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-865">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-866">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-866">Keyvault</span></span>

* <span data-ttu-id="a8ca3-867">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="a8ca3-867">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-868">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-868">VM</span></span>

* <span data-ttu-id="a8ca3-869">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-869">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a8ca3-870">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="a8ca3-870">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a8ca3-871">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-871">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a8ca3-872">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-872">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a8ca3-873">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-873">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a8ca3-874">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-874">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-875">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-875">ACS</span></span>

* <span data-ttu-id="a8ca3-876">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="a8ca3-876">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-877">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-877">Appservice</span></span>

* <span data-ttu-id="a8ca3-878">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-878">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a8ca3-879">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a8ca3-879">Backup</span></span>

* <span data-ttu-id="a8ca3-880">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-880">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a8ca3-881">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-881">September 11, 2017</span></span>

<span data-ttu-id="a8ca3-882">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a8ca3-882">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a8ca3-883">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-883">Core</span></span>

* <span data-ttu-id="a8ca3-884">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-884">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a8ca3-885">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="a8ca3-885">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-886">Acs</span><span class="sxs-lookup"><span data-stu-id="a8ca3-886">Acs</span></span>

* <span data-ttu-id="a8ca3-887">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-887">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a8ca3-888">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="a8ca3-888">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-889">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-889">Appservice</span></span>

* <span data-ttu-id="a8ca3-890">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-890">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a8ca3-891">CDN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-891">CDN</span></span>

* <span data-ttu-id="a8ca3-892">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-892">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a8ca3-893">Extension</span><span class="sxs-lookup"><span data-stu-id="a8ca3-893">Extension</span></span>

* <span data-ttu-id="a8ca3-894">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-894">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-895">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-895">Keyvault</span></span>

* <span data-ttu-id="a8ca3-896">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-896">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-897">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-897">Network</span></span>

* <span data-ttu-id="a8ca3-898">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-898">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a8ca3-899">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-899">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a8ca3-900">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-900">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a8ca3-901">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-901">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a8ca3-902">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-902">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-903">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-903">Resource</span></span>

* <span data-ttu-id="a8ca3-904">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-904">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a8ca3-905">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-905">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a8ca3-906">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="a8ca3-906">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a8ca3-907">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="a8ca3-907">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-908">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-908">SQL</span></span>

* <span data-ttu-id="a8ca3-909">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-909">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-910">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-910">VM</span></span>

* <span data-ttu-id="a8ca3-911">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="a8ca3-911">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a8ca3-912">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-912">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a8ca3-913">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-913">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a8ca3-914">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="a8ca3-914">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a8ca3-915">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="a8ca3-915">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a8ca3-916">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-916">August 31, 2017</span></span>

<span data-ttu-id="a8ca3-917">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a8ca3-917">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-918">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-918">Keyvault</span></span>

* <span data-ttu-id="a8ca3-919">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-919">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a8ca3-920">Sf</span><span class="sxs-lookup"><span data-stu-id="a8ca3-920">Sf</span></span>

* <span data-ttu-id="a8ca3-921">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-921">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-922">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-922">Storage</span></span>

* <span data-ttu-id="a8ca3-923">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="a8ca3-923">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a8ca3-924">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-924">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a8ca3-925">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-925">August 28, 2017</span></span>

<span data-ttu-id="a8ca3-926">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a8ca3-926">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a8ca3-927">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-927">CLI</span></span>

* <span data-ttu-id="a8ca3-928">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-928">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-929">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-929">ACS</span></span>

* <span data-ttu-id="a8ca3-930">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a8ca3-930">Corrected preview regions</span></span>
* <span data-ttu-id="a8ca3-931">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-931">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a8ca3-932">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-932">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-933">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-933">Appservice</span></span>

* <span data-ttu-id="a8ca3-934">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-934">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a8ca3-935">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-935">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a8ca3-936">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-936">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a8ca3-937">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-937">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a8ca3-938">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-938">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-939">IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-939">IoT</span></span>

* <span data-ttu-id="a8ca3-940">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-940">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-941">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-941">Network</span></span>

* <span data-ttu-id="a8ca3-942">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-942">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a8ca3-943">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-943">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a8ca3-944">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-944">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a8ca3-945">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-945">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a8ca3-946">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-946">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-947">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-947">Profile</span></span>

* <span data-ttu-id="a8ca3-948">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-948">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a8ca3-949">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a8ca3-949">Service Fabric</span></span>

* <span data-ttu-id="a8ca3-950">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-950">Preview release</span></span>
* <span data-ttu-id="a8ca3-951">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-951">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a8ca3-952">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="a8ca3-952">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a8ca3-953">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-953">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-954">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-954">Storage</span></span>

* <span data-ttu-id="a8ca3-955">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="a8ca3-955">Enabled setting blob tier</span></span>
* <span data-ttu-id="a8ca3-956">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="a8ca3-956">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a8ca3-957">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-957">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a8ca3-958">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="a8ca3-958">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a8ca3-959">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-959">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a8ca3-960">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-960">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-961">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-961">VM</span></span>

* <span data-ttu-id="a8ca3-962">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-962">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a8ca3-963">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="a8ca3-963">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a8ca3-964">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-964">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a8ca3-965">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="a8ca3-965">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a8ca3-966">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="a8ca3-966">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a8ca3-967">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-967">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a8ca3-968">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-968">August 15, 2017</span></span>

<span data-ttu-id="a8ca3-969">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a8ca3-969">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-970">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-970">ACS</span></span>

* <span data-ttu-id="a8ca3-971">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-971">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-972">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-972">Appservice</span></span>

* <span data-ttu-id="a8ca3-973">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="a8ca3-973">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a8ca3-974">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a8ca3-974">Event Grid</span></span>

* <span data-ttu-id="a8ca3-975">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-975">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a8ca3-976">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-976">August 11, 2017</span></span>

<span data-ttu-id="a8ca3-977">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a8ca3-977">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-978">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-978">ACS</span></span>

* <span data-ttu-id="a8ca3-979">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a8ca3-979">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-980">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-980">Batch</span></span>

* <span data-ttu-id="a8ca3-981">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-981">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a8ca3-982">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-982">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a8ca3-983">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="a8ca3-983">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a8ca3-984">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-984">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a8ca3-985">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="a8ca3-985">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a8ca3-986">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-986">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a8ca3-987">Composant</span><span class="sxs-lookup"><span data-stu-id="a8ca3-987">Component</span></span>

* <span data-ttu-id="a8ca3-988">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-988">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a8ca3-989">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-989">Container</span></span>

* <span data-ttu-id="a8ca3-990">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-990">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a8ca3-991">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-991">Data Lake Store</span></span>

* <span data-ttu-id="a8ca3-992">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="a8ca3-992">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a8ca3-993">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a8ca3-993">Event Grid</span></span>

* <span data-ttu-id="a8ca3-994">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a8ca3-994">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-995">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-995">Network</span></span>

* <span data-ttu-id="a8ca3-996">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="a8ca3-996">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a8ca3-997">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-997">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a8ca3-998">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="a8ca3-998">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a8ca3-999">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-999">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-1000">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1000">Profile</span></span>

* <span data-ttu-id="a8ca3-1001">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1001">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-1002">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1002">Storage</span></span>

* <span data-ttu-id="a8ca3-1003">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1003">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-1004">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1004">VM</span></span>

* <span data-ttu-id="a8ca3-1005">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1005">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a8ca3-1006">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1006">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a8ca3-1007">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1007">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a8ca3-1008">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1008">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a8ca3-1009">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1009">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a8ca3-1010">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1010">July 28, 2017</span></span>

<span data-ttu-id="a8ca3-1011">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1011">Version 2.0.12</span></span>

* <span data-ttu-id="a8ca3-1012">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1012">Added container commands</span></span>
* <span data-ttu-id="a8ca3-1013">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1013">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a8ca3-1014">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1014">Core</span></span>

* <span data-ttu-id="a8ca3-1015">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1015">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a8ca3-1016">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1016">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a8ca3-1017">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1017">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a8ca3-1018">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1018">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a8ca3-1019">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1019">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a8ca3-1020">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1020">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a8ca3-1021">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1021">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a8ca3-1022">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1022">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a8ca3-1023">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1023">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a8ca3-1024">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1024">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a8ca3-1025">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1025">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a8ca3-1026">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1026">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a8ca3-1027">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1027">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a8ca3-1028">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1028">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a8ca3-1029">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1029">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a8ca3-1030">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1030">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a8ca3-1031">ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1031">ACR</span></span>

* <span data-ttu-id="a8ca3-1032">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1032">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a8ca3-1033">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1033">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a8ca3-1034">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1034">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a8ca3-1035">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1035">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a8ca3-1036">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1036">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a8ca3-1037">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1037">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-1038">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1038">ACS</span></span>

* <span data-ttu-id="a8ca3-1039">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1039">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-1040">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1040">Appservice</span></span>

* <span data-ttu-id="a8ca3-1041">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1041">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a8ca3-1042">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1042">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a8ca3-1043">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1043">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a8ca3-1044">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1044">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a8ca3-1045">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1045">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a8ca3-1046">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1046">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a8ca3-1047">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1047">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a8ca3-1048">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1048">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a8ca3-1049">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1049">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a8ca3-1050">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1050">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a8ca3-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1051">Batch</span></span>

* <span data-ttu-id="a8ca3-1052">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1052">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a8ca3-1053">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1053">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a8ca3-1054">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1054">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a8ca3-1055">CDN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1055">CDN</span></span>

* <span data-ttu-id="a8ca3-1056">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1056">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a8ca3-1057">Cloud</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1057">Cloud</span></span>

* <span data-ttu-id="a8ca3-1058">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1058">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a8ca3-1059">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1059">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a8ca3-1060">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1060">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a8ca3-1061">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1061">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a8ca3-1062">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1062">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a8ca3-1063">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1063">CosmosDB</span></span>

* <span data-ttu-id="a8ca3-1064">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1064">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a8ca3-1065">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1065">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a8ca3-1066">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1066">Data Lake Analytics</span></span>

* <span data-ttu-id="a8ca3-1067">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1067">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a8ca3-1068">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1068">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a8ca3-1069">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1069">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a8ca3-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1070">Data Lake Store</span></span>

* <span data-ttu-id="a8ca3-1071">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1071">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a8ca3-1072">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1072">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a8ca3-1073">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1073">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a8ca3-1074">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1074">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a8ca3-1075">Interactive</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1075">Interactive</span></span>

* <span data-ttu-id="a8ca3-1076">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1076">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a8ca3-1077">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1077">Increased test coverage</span></span>
* <span data-ttu-id="a8ca3-1078">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1078">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a8ca3-1079">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1079">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a8ca3-1080">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1080">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a8ca3-1081">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1081">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a8ca3-1082">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1082">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a8ca3-1083">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1083">Added `--progress` flag</span></span>
* <span data-ttu-id="a8ca3-1084">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1084">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a8ca3-1085">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1085">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a8ca3-1086">IoT</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1086">IoT</span></span>

* <span data-ttu-id="a8ca3-1087">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1087">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a8ca3-1088">(#3934)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1088">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a8ca3-1089">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1089">Key vault</span></span>

* <span data-ttu-id="a8ca3-1090">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1090">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a8ca3-1091">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1091">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a8ca3-1092">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1092">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a8ca3-1093">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1093">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a8ca3-1094">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1094">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a8ca3-1095">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1095">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a8ca3-1096">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1096">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a8ca3-1097">(#3307)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1097">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a8ca3-1098">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1098">Lab</span></span>

* <span data-ttu-id="a8ca3-1099">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1099">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a8ca3-1100">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1100">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-1101">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1101">Monitor</span></span>

* <span data-ttu-id="a8ca3-1102">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1102">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a8ca3-1103">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1103">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a8ca3-1104">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1104">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a8ca3-1105">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1105">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a8ca3-1106">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1106">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a8ca3-1107">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1107">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a8ca3-1108">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1108">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a8ca3-1109">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1109">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a8ca3-1110">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1110">`location` no longer required</span></span>
  * <span data-ttu-id="a8ca3-1111">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1111">Add name and ID support for target</span></span>
  * <span data-ttu-id="a8ca3-1112">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1112">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a8ca3-1113">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1113">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a8ca3-1114">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1114">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a8ca3-1115">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1115">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a8ca3-1116">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1116">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a8ca3-1117">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1117">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-1118">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1118">Network</span></span>

* <span data-ttu-id="a8ca3-1119">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1119">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a8ca3-1120">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1120">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a8ca3-1121">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1121">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a8ca3-1122">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1122">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a8ca3-1123">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1123">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a8ca3-1124">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1124">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a8ca3-1125">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1125">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a8ca3-1126">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1126">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a8ca3-1127">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1127">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a8ca3-1128">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1128">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a8ca3-1129">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1129">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a8ca3-1130">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1130">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a8ca3-1131">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1131">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a8ca3-1132">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1132">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a8ca3-1133">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1133">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a8ca3-1134">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1134">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a8ca3-1135">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1135">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a8ca3-1136">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1136">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a8ca3-1137">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1137">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a8ca3-1138">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1138">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a8ca3-1139">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1139">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a8ca3-1140">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1140">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a8ca3-1141">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1141">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a8ca3-1142">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1142">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a8ca3-1143">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1143">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a8ca3-1144">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1144">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a8ca3-1145">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1145">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-1146">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1146">Profile</span></span>

* <span data-ttu-id="a8ca3-1147">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1147">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a8ca3-1148">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1148">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a8ca3-1149">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1149">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a8ca3-1150">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1150">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a8ca3-1151">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1151">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a8ca3-1152">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1152">RDBMS</span></span>

* <span data-ttu-id="a8ca3-1153">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1153">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a8ca3-1154">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1154">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a8ca3-1155">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1155">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a8ca3-1156">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1156">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-1157">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1157">Resource</span></span>

* <span data-ttu-id="a8ca3-1158">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1158">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a8ca3-1159">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1159">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a8ca3-1160">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1160">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a8ca3-1161">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1161">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a8ca3-1162">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1162">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a8ca3-1163">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1163">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a8ca3-1164">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1164">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a8ca3-1165">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1165">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-1166">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1166">Role</span></span>

* <span data-ttu-id="a8ca3-1167">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1167">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a8ca3-1168">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1168">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a8ca3-1169">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1169">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a8ca3-1170">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1170">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a8ca3-1171">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1171">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a8ca3-1172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1172">Service Fabric</span></span>
* <span data-ttu-id="a8ca3-1173">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1173">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a8ca3-1174">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1174">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a8ca3-1175">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1175">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-1176">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1176">SQL</span></span>

* <span data-ttu-id="a8ca3-1177">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1177">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a8ca3-1178">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1178">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a8ca3-1179">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1179">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-1180">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1180">Storage</span></span>

* <span data-ttu-id="a8ca3-1181">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1181">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a8ca3-1182">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1182">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a8ca3-1183">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1183">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a8ca3-1184">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1184">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a8ca3-1185">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1185">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a8ca3-1186">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1186">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-1187">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1187">VM</span></span>

* <span data-ttu-id="a8ca3-1188">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1188">Support configuring nsg</span></span>
* <span data-ttu-id="a8ca3-1189">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1189">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a8ca3-1190">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1190">Support managed service identities</span></span>
* <span data-ttu-id="a8ca3-1191">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1191">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a8ca3-1192">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1192">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a8ca3-1193">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1193">May 10, 2017</span></span>

<span data-ttu-id="a8ca3-1194">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1194">Version 2.0.6</span></span>

* <span data-ttu-id="a8ca3-1195">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1195">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a8ca3-1196">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1196">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a8ca3-1197">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1197">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a8ca3-1198">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1198">Include Cognitive Services module</span></span>
* <span data-ttu-id="a8ca3-1199">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1199">Include Service Fabric module</span></span>
* <span data-ttu-id="a8ca3-1200">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1200">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a8ca3-1201">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1201">Add support for CDN commands</span></span>
* <span data-ttu-id="a8ca3-1202">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1202">Remove Container module</span></span>
* <span data-ttu-id="a8ca3-1203">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1203">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a8ca3-1204">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1204">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a8ca3-1205">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1205">Core</span></span>

* <span data-ttu-id="a8ca3-1206">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1206">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a8ca3-1207">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1207">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a8ca3-1208">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1208">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a8ca3-1209">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1209">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a8ca3-1210">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1210">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a8ca3-1211">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1211">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a8ca3-1212">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1212">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a8ca3-1213">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1213">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a8ca3-1214">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1214">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a8ca3-1215">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1215">core: Improved performance</span></span>
* <span data-ttu-id="a8ca3-1216">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1216">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a8ca3-1217">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1217">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-1218">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1218">ACS</span></span>

* <span data-ttu-id="a8ca3-1219">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1219">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a8ca3-1220">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1220">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a8ca3-1221">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1221">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a8ca3-1222">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1222">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-1223">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1223">AppService</span></span>

* <span data-ttu-id="a8ca3-1224">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1224">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a8ca3-1225">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1225">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a8ca3-1226">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1226">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a8ca3-1227">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1227">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a8ca3-1228">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1228">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a8ca3-1229">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1229">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a8ca3-1230">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1230">support slot swap with preview</span></span>
* <span data-ttu-id="a8ca3-1231">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1231">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a8ca3-1232">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1232">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a8ca3-1233">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1233">CosmosDB</span></span>

* <span data-ttu-id="a8ca3-1234">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1234">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a8ca3-1235">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1235">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a8ca3-1236">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1236">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a8ca3-1237">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1237">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a8ca3-1238">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1238">Data Lake Analytics</span></span>

* <span data-ttu-id="a8ca3-1239">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1239">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a8ca3-1240">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1240">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a8ca3-1241">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1241">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a8ca3-1242">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1242">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a8ca3-1243">Table</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1243">Table</span></span>
  * <span data-ttu-id="a8ca3-1244">Fonction table</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1244">Table valued function</span></span>
  * <span data-ttu-id="a8ca3-1245">Affichage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1245">View</span></span>
  * <span data-ttu-id="a8ca3-1246">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1246">Table Statistics.</span></span> <span data-ttu-id="a8ca3-1247">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1247">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a8ca3-1248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1248">Data Lake Store</span></span>

* <span data-ttu-id="a8ca3-1249">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1249">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a8ca3-1250">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1250">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a8ca3-1251">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1251">missed help for access show.</span></span> <span data-ttu-id="a8ca3-1252">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1252">adding it.</span></span> <span data-ttu-id="a8ca3-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a8ca3-1254">Rechercher</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1254">Find</span></span>

* <span data-ttu-id="a8ca3-1255">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1255">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a8ca3-1256">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1256">KeyVault</span></span>

* <span data-ttu-id="a8ca3-1257">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1257">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a8ca3-1258">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1258">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a8ca3-1259">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1259">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a8ca3-1260">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1260">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a8ca3-1261">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1261">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a8ca3-1262">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1262">Lab</span></span>

* <span data-ttu-id="a8ca3-1263">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1263">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a8ca3-1264">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1264">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a8ca3-1265">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1265">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a8ca3-1266">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1266">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a8ca3-1267">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1267">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a8ca3-1268">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1268">Monitor</span></span>

* <span data-ttu-id="a8ca3-1269">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1269">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a8ca3-1270">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1270">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a8ca3-1271">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1271">Network</span></span>

* <span data-ttu-id="a8ca3-1272">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1272">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a8ca3-1273">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1273">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a8ca3-1274">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1274">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a8ca3-1275">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1275">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a8ca3-1276">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1276">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a8ca3-1277">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1277">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a8ca3-1278">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1278">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a8ca3-1279">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1279">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a8ca3-1280">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1280">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a8ca3-1281">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1281">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a8ca3-1282">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1282">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a8ca3-1283">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1283">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a8ca3-1284">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1284">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a8ca3-1285">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1285">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a8ca3-1286">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1286">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a8ca3-1287">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1287">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a8ca3-1288">Profil</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1288">Profile</span></span>

* <span data-ttu-id="a8ca3-1289">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1289">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a8ca3-1290">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1290">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a8ca3-1291">Redis</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1291">Redis</span></span>

* <span data-ttu-id="a8ca3-1292">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1292">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a8ca3-1293">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1293">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a8ca3-1294">Ressource</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1294">Resource</span></span>

* <span data-ttu-id="a8ca3-1295">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1295">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a8ca3-1296">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1296">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a8ca3-1297">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1297">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a8ca3-1298">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1298">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a8ca3-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a8ca3-1300">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1300">Add docs for az lock update.</span></span> <span data-ttu-id="a8ca3-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a8ca3-1302">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1302">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a8ca3-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a8ca3-1304">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1304">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a8ca3-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a8ca3-1306">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1306">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a8ca3-1307">Rôle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1307">Role</span></span>

* <span data-ttu-id="a8ca3-1308">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1308">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a8ca3-1309">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1309">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a8ca3-1310">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1310">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a8ca3-1311">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1311">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a8ca3-1312">SQL</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1312">SQL</span></span>

* <span data-ttu-id="a8ca3-1313">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1313">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a8ca3-1314">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1314">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a8ca3-1315">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1315">Storage</span></span>

* <span data-ttu-id="a8ca3-1316">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1316">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a8ca3-1317">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1317">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a8ca3-1318">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1318">Add support for large block blob upload</span></span>
* <span data-ttu-id="a8ca3-1319">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1319">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-1320">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1320">VM</span></span>

* <span data-ttu-id="a8ca3-1321">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1321">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a8ca3-1322">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1322">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a8ca3-1323">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1323">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a8ca3-1324">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1324">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a8ca3-1325">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1325">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a8ca3-1326">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1326">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a8ca3-1327">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1327">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a8ca3-1328">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1328">April 3, 2017</span></span>

<span data-ttu-id="a8ca3-1329">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1329">Version 2.0.2</span></span>

<span data-ttu-id="a8ca3-1330">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1330">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a8ca3-1331">Principal</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1331">Core</span></span>

* <span data-ttu-id="a8ca3-1332">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1332">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a8ca3-1333">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1333">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a8ca3-1334">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1334">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a8ca3-1335">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1335">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a8ca3-1336">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1336">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a8ca3-1337">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1337">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a8ca3-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a8ca3-1339">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1339">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a8ca3-1340">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1340">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a8ca3-1341">ACS</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1341">ACS</span></span>

* <span data-ttu-id="a8ca3-1342">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1342">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a8ca3-1343">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1343">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a8ca3-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a8ca3-1345">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1345">Add support for windows clusters.</span></span> <span data-ttu-id="a8ca3-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a8ca3-1347">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1347">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a8ca3-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a8ca3-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1349">AppService</span></span>

* <span data-ttu-id="a8ca3-1350">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1350">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a8ca3-1351">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1351">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a8ca3-1352">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1352">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a8ca3-1353">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1353">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a8ca3-1354">DataLake</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1354">DataLake</span></span>

* <span data-ttu-id="a8ca3-1355">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1355">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a8ca3-1356">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1356">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a8ca3-1357">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1357">DocuemntDB</span></span>

* <span data-ttu-id="a8ca3-1358">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1358">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a8ca3-1359">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1359">VM</span></span>

* <span data-ttu-id="a8ca3-1360">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1360">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a8ca3-1361">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1361">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a8ca3-1362">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1362">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a8ca3-1363">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1363">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a8ca3-1364">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1364">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a8ca3-1365">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1365">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="a8ca3-1366">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1366">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a8ca3-1367">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1367">February 27, 2017</span></span>

<span data-ttu-id="a8ca3-1368">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1368">Version 2.0.0</span></span>

<span data-ttu-id="a8ca3-1369">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1369">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a8ca3-1370">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1370">Container Service (acs)</span></span>
- <span data-ttu-id="a8ca3-1371">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1371">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a8ca3-1372">Réseau</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1372">Networking</span></span>
- <span data-ttu-id="a8ca3-1373">Stockage</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1373">Storage</span></span>

<span data-ttu-id="a8ca3-1374">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1374">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a8ca3-1375">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1375">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a8ca3-1376">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1376">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a8ca3-1377">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1377">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a8ca3-1378">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1378">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a8ca3-1379">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1379">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a8ca3-1380">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1380">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a8ca3-1381">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1381">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a8ca3-1382">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a8ca3-1382">Provide feedback from the command line with the `az feedback` command</span></span>

