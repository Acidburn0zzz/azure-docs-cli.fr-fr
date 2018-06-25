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
ms.openlocfilehash: 64db2b58ca883518757d8e189bf7263ed818b283
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262656"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="77ea9-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="77ea9-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="77ea9-104">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-104">June 19, 2018</span></span>

<span data-ttu-id="77ea9-105">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="77ea9-105">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-106">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-106">Core</span></span>

* <span data-ttu-id="77ea9-107">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-107">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-108">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-108">ACR</span></span>

* <span data-ttu-id="77ea9-109">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="77ea9-109">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="77ea9-110">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-110">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-111">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-111">ACS</span></span>

* <span data-ttu-id="77ea9-112">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-112">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="77ea9-113">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-113">Added `--update` support</span></span>
* <span data-ttu-id="77ea9-114">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="77ea9-114">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="77ea9-115">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="77ea9-115">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="77ea9-116">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="77ea9-116">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="77ea9-117">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="77ea9-117">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="77ea9-118">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="77ea9-118">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="77ea9-119">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="77ea9-119">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span> 

### <a name="appservice"></a><span data-ttu-id="77ea9-120">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-120">AppService</span></span>

* <span data-ttu-id="77ea9-121">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="77ea9-121">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="77ea9-122">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="77ea9-122">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-123">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-123">Batch</span></span>

* <span data-ttu-id="77ea9-124">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="77ea9-124">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="77ea9-125">Batch AI</span><span class="sxs-lookup"><span data-stu-id="77ea9-125">Batch AI</span></span>

* <span data-ttu-id="77ea9-126">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="77ea9-126">Added support for workspaces.</span></span> <span data-ttu-id="77ea9-127">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="77ea9-127">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="77ea9-128">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="77ea9-128">Added support for experiments.</span></span> <span data-ttu-id="77ea9-129">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="77ea9-129">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="77ea9-130">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="77ea9-130">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="77ea9-131">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-131">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="77ea9-132">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="77ea9-132">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="77ea9-133">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="77ea9-133">Added support for `--ids` to `batchai` commands</span></span> 
* <span data-ttu-id="77ea9-134">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-134">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="77ea9-135">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="77ea9-135">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="77ea9-136">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-136">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="77ea9-137">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="77ea9-137">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="77ea9-138">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-138">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="77ea9-139">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="77ea9-139">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="77ea9-140">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="77ea9-140">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="77ea9-141">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="77ea9-141">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="77ea9-142">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-142">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="77ea9-143">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="77ea9-143">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="77ea9-144">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="77ea9-144">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="77ea9-145">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="77ea9-145">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="77ea9-146">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="77ea9-146">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="77ea9-147">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="77ea9-147">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="77ea9-148">Cartes</span><span class="sxs-lookup"><span data-stu-id="77ea9-148">Maps</span></span>

* <span data-ttu-id="77ea9-149">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="77ea9-149">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-150">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-150">Network</span></span>

* <span data-ttu-id="77ea9-151">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="77ea9-151">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="77ea9-152">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="77ea9-152">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="77ea9-153">#6502</span><span class="sxs-lookup"><span data-stu-id="77ea9-153">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="77ea9-154">Réservations</span><span class="sxs-lookup"><span data-stu-id="77ea9-154">Reservations</span></span>

* <span data-ttu-id="77ea9-155">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-155">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="77ea9-156">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-156">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="77ea9-157">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="77ea9-157">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="77ea9-158">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="77ea9-158">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="77ea9-159">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="77ea9-159">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="77ea9-160">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-160">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-161">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-161">Role</span></span>

* <span data-ttu-id="77ea9-162">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-162">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-163">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-163">SQL</span></span>

* <span data-ttu-id="77ea9-164">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="77ea9-164">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-165">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-165">Storage</span></span>

* <span data-ttu-id="77ea9-166">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="77ea9-166">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-167">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-167">VM</span></span>

* <span data-ttu-id="77ea9-168">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-168">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="77ea9-169">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="77ea9-169">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="77ea9-170">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="77ea9-170">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="77ea9-171">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-171">June 13, 2018</span></span>

<span data-ttu-id="77ea9-172">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="77ea9-172">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-173">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-173">Core</span></span>

* <span data-ttu-id="77ea9-174">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-174">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="77ea9-175">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-175">June 13, 2018</span></span>

<span data-ttu-id="77ea9-176">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="77ea9-176">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="77ea9-177">AKS</span><span class="sxs-lookup"><span data-stu-id="77ea9-177">AKS</span></span>

* <span data-ttu-id="77ea9-178">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-178">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="77ea9-179">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="77ea9-179">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="77ea9-180">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-180">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="77ea9-181">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-181">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="77ea9-182">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-182">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-183">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-183">AppService</span></span>

* <span data-ttu-id="77ea9-184">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="77ea9-184">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="77ea9-185">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-185">June 5, 2018</span></span>

<span data-ttu-id="77ea9-186">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="77ea9-186">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-187">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-187">Interactive</span></span>

* <span data-ttu-id="77ea9-188">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="77ea9-188">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="77ea9-189">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-189">June 5, 2018</span></span>

<span data-ttu-id="77ea9-190">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="77ea9-190">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-191">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-191">Core</span></span>

* <span data-ttu-id="77ea9-192">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="77ea9-192">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="77ea9-193">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="77ea9-193">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-194">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-194">ACR</span></span>

* <span data-ttu-id="77ea9-195">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="77ea9-195">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="77ea9-196">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="77ea9-196">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="77ea9-197">AKS</span><span class="sxs-lookup"><span data-stu-id="77ea9-197">AKS</span></span>

* <span data-ttu-id="77ea9-198">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="77ea9-198">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-199">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-199">Batch</span></span>

* <span data-ttu-id="77ea9-200">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="77ea9-200">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-201">IOT</span><span class="sxs-lookup"><span data-stu-id="77ea9-201">IOT</span></span>

* <span data-ttu-id="77ea9-202">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="77ea9-202">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-203">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-203">Network</span></span>

* <span data-ttu-id="77ea9-204">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="77ea9-204">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="77ea9-205">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="77ea9-205">Policy Insights</span></span>

* <span data-ttu-id="77ea9-206">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-206">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="77ea9-207">ARM</span><span class="sxs-lookup"><span data-stu-id="77ea9-207">ARM</span></span>

* <span data-ttu-id="77ea9-208">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-208">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-209">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-209">SQL</span></span>

* <span data-ttu-id="77ea9-210">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="77ea9-210">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="77ea9-211">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="77ea9-211">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="77ea9-212">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-212">Storage</span></span>

* <span data-ttu-id="77ea9-213">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="77ea9-213">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-214">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-214">VM</span></span>

* <span data-ttu-id="77ea9-215">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="77ea9-215">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="77ea9-216">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-216">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="77ea9-217">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-217">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="77ea9-218">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-218">May 22, 2018</span></span>

<span data-ttu-id="77ea9-219">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="77ea9-219">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-220">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-220">Core</span></span>

* <span data-ttu-id="77ea9-221">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="77ea9-221">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-222">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-222">ACS</span></span>

* <span data-ttu-id="77ea9-223">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="77ea9-223">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="77ea9-224">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="77ea9-224">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-225">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-225">AppService</span></span>

* <span data-ttu-id="77ea9-226">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="77ea9-226">Improved generic update commands</span></span>
* <span data-ttu-id="77ea9-227">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="77ea9-227">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-228">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-228">Container</span></span>

* <span data-ttu-id="77ea9-229">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="77ea9-229">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="77ea9-230">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-230">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-231">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-231">Extension</span></span>

* <span data-ttu-id="77ea9-232">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="77ea9-232">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-233">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-233">Interactive</span></span>

* <span data-ttu-id="77ea9-234">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="77ea9-234">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="77ea9-235">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="77ea9-235">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-236">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-236">KeyVault</span></span>

* <span data-ttu-id="77ea9-237">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="77ea9-237">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-238">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-238">Network</span></span>

* <span data-ttu-id="77ea9-239">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="77ea9-239">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="77ea9-240">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="77ea9-240">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-241">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-241">SQL</span></span>

* <span data-ttu-id="77ea9-242">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="77ea9-242">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="77ea9-243">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="77ea9-243">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="77ea9-244">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="77ea9-244">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="77ea9-245">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="77ea9-245">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="77ea9-246">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="77ea9-246">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="77ea9-247">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-247">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="77ea9-248">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-248">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="77ea9-249">`edition`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-249">`edition`.</span></span> <span data-ttu-id="77ea9-250">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="77ea9-250">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="77ea9-251">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-251">`elasticPoolName`.</span></span> <span data-ttu-id="77ea9-252">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="77ea9-252">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="77ea9-253">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="77ea9-253">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="77ea9-254">`edition`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-254">`edition`.</span></span> <span data-ttu-id="77ea9-255">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="77ea9-255">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="77ea9-256">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-256">`dtu`.</span></span> <span data-ttu-id="77ea9-257">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="77ea9-257">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="77ea9-258">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-258">`databaseDtuMin`.</span></span> <span data-ttu-id="77ea9-259">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="77ea9-259">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="77ea9-260">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-260">`databaseDtuMax`.</span></span> <span data-ttu-id="77ea9-261">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="77ea9-261">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="77ea9-262">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="77ea9-262">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="77ea9-263">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="77ea9-263">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-264">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-264">Storage</span></span>

* <span data-ttu-id="77ea9-265">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-265">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="77ea9-266">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="77ea9-266">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-267">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-267">VM</span></span>

* <span data-ttu-id="77ea9-268">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-268">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="77ea9-269">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="77ea9-269">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="77ea9-270">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="77ea9-270">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="77ea9-271">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="77ea9-271">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="77ea9-272">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-272">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="77ea9-273">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-273">May 7, 2018</span></span>

<span data-ttu-id="77ea9-274">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="77ea9-274">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-275">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-275">Core</span></span>

* <span data-ttu-id="77ea9-276">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="77ea9-276">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="77ea9-277">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="77ea9-277">Added limited support for positional arguments</span></span>
* <span data-ttu-id="77ea9-278">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-278">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="77ea9-279">#5591</span><span class="sxs-lookup"><span data-stu-id="77ea9-279">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="77ea9-280">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-280">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="77ea9-281">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="77ea9-281">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="77ea9-282">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-282">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="77ea9-283">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="77ea9-283">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="77ea9-284">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-284">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-285">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-285">ACR</span></span>

* <span data-ttu-id="77ea9-286">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-286">Added ACR Build commands</span></span>
* <span data-ttu-id="77ea9-287">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="77ea9-287">Improved resource not found error messages</span></span>
* <span data-ttu-id="77ea9-288">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-288">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="77ea9-289">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="77ea9-289">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="77ea9-290">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="77ea9-290">Improved repository commands error messages</span></span>
* <span data-ttu-id="77ea9-291">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="77ea9-291">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-292">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-292">ACS</span></span>

* <span data-ttu-id="77ea9-293">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="77ea9-293">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="77ea9-294">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="77ea9-294">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="77ea9-295">AMS</span><span class="sxs-lookup"><span data-stu-id="77ea9-295">AMS</span></span>

* <span data-ttu-id="77ea9-296">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="77ea9-296">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-297">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-297">Appservice</span></span>

* <span data-ttu-id="77ea9-298">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="77ea9-298">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="77ea9-299">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-299">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="77ea9-300">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="77ea9-300">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="77ea9-301">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-301">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="77ea9-302">Batch AI</span><span class="sxs-lookup"><span data-stu-id="77ea9-302">Batch AI</span></span>

* <span data-ttu-id="77ea9-303">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="77ea9-303">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="77ea9-304">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="77ea9-304">Cognitive Services</span></span>

* <span data-ttu-id="77ea9-305">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="77ea9-305">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="77ea9-306">Consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-306">Consumption</span></span>

* <span data-ttu-id="77ea9-307">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="77ea9-307">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-308">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-308">Container</span></span>

* <span data-ttu-id="77ea9-309">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="77ea9-309">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="77ea9-310">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="77ea9-310">Cosmos DB</span></span>

* <span data-ttu-id="77ea9-311">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="77ea9-311">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="77ea9-312">DMS</span><span class="sxs-lookup"><span data-stu-id="77ea9-312">DMS</span></span>

* <span data-ttu-id="77ea9-313">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="77ea9-313">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-314">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-314">Extension</span></span>

* <span data-ttu-id="77ea9-315">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="77ea9-315">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-316">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-316">Interactive</span></span>

* <span data-ttu-id="77ea9-317">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="77ea9-317">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="77ea9-318">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="77ea9-318">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="77ea9-319">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="77ea9-319">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="77ea9-320">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-320">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="77ea9-321">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-321">Lab</span></span>

* <span data-ttu-id="77ea9-322">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="77ea9-322">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-323">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-323">Network</span></span>

* <span data-ttu-id="77ea9-324">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="77ea9-324">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="77ea9-325">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-325">Profile</span></span>

* <span data-ttu-id="77ea9-326">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-326">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="77ea9-327">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="77ea9-327">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="77ea9-328">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="77ea9-328">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="77ea9-329">Redis</span><span class="sxs-lookup"><span data-stu-id="77ea9-329">Redis</span></span>

* <span data-ttu-id="77ea9-330">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-330">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="77ea9-331">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="77ea9-331">Deprecated `redis list-all`.</span></span> <span data-ttu-id="77ea9-332">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-332">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="77ea9-333">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="77ea9-333">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="77ea9-334">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-334">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-335">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-335">Role</span></span>

* <span data-ttu-id="77ea9-336">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="77ea9-336">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-337">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-337">Storage</span></span>

* <span data-ttu-id="77ea9-338">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="77ea9-338">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="77ea9-339">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="77ea9-339">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="77ea9-340">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="77ea9-340">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="77ea9-341">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="77ea9-341">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="77ea9-342">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-342">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-343">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-343">VM</span></span>

* <span data-ttu-id="77ea9-344">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="77ea9-344">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="77ea9-345">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="77ea9-345">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="77ea9-346">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="77ea9-346">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="77ea9-347">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="77ea9-347">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="77ea9-348">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="77ea9-348">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="77ea9-349">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="77ea9-349">Added write accelerator support</span></span> 
* <span data-ttu-id="77ea9-350">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="77ea9-350">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="77ea9-351">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-351">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="77ea9-352">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="77ea9-352">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="77ea9-353">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-353">April 10, 2018</span></span>

<span data-ttu-id="77ea9-354">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="77ea9-354">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-355">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-355">ACR</span></span>

* <span data-ttu-id="77ea9-356">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="77ea9-356">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-357">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-357">ACS</span></span>

* <span data-ttu-id="77ea9-358">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="77ea9-358">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-359">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-359">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="77ea9-361">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="77ea9-361">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="77ea9-362">Batch AI</span><span class="sxs-lookup"><span data-stu-id="77ea9-362">BatchAI</span></span>

* <span data-ttu-id="77ea9-363">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="77ea9-363">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="77ea9-364">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-364">Job level mounting</span></span>
 - <span data-ttu-id="77ea9-365">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="77ea9-365">Environment variables with secret values</span></span>
 - <span data-ttu-id="77ea9-366">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="77ea9-366">Performance counters settings</span></span>
 - <span data-ttu-id="77ea9-367">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-367">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="77ea9-368">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="77ea9-368">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="77ea9-369">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="77ea9-369">Usage and limits reporting</span></span>
 - <span data-ttu-id="77ea9-370">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="77ea9-370">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="77ea9-371">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="77ea9-371">Support for custom images</span></span>
 - <span data-ttu-id="77ea9-372">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="77ea9-372">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="77ea9-373">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-373">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="77ea9-374">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="77ea9-374">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="77ea9-375">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="77ea9-375">National clouds are supported</span></span>
* <span data-ttu-id="77ea9-376">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="77ea9-376">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="77ea9-377">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="77ea9-377">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="77ea9-378">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="77ea9-378">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="77ea9-379">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="77ea9-379">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="77ea9-380">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="77ea9-380">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="77ea9-381">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="77ea9-381">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="77ea9-382">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-382">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="77ea9-383">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="77ea9-383">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="77ea9-384">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="77ea9-384">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="77ea9-385">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-385">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="77ea9-386">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-386">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="77ea9-387">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="77ea9-387">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="77ea9-388">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-388">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="77ea9-389">Facturation</span><span class="sxs-lookup"><span data-stu-id="77ea9-389">Billing</span></span>

* <span data-ttu-id="77ea9-390">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="77ea9-390">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="77ea9-391">Consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-391">Consumption</span></span>

* <span data-ttu-id="77ea9-392">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="77ea9-392">Added `marketplace` commands</span></span>
* <span data-ttu-id="77ea9-393">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="77ea9-393">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="77ea9-394">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="77ea9-394">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="77ea9-395">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="77ea9-395">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="77ea9-396">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="77ea9-396">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="77ea9-397">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="77ea9-397">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-398">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-398">Container</span></span>

* <span data-ttu-id="77ea9-399">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="77ea9-399">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="77ea9-400">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="77ea9-400">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-401">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-401">Extension</span></span>

* <span data-ttu-id="77ea9-402">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="77ea9-402">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-403">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-403">Interactive</span></span>

* <span data-ttu-id="77ea9-404">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="77ea9-404">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="77ea9-405">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-405">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="77ea9-406">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="77ea9-406">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-407">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-407">Network</span></span>

* <span data-ttu-id="77ea9-408">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="77ea9-408">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="77ea9-409">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-409">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="77ea9-410">#4910</span><span class="sxs-lookup"><span data-stu-id="77ea9-410">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="77ea9-411">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="77ea9-411">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="77ea9-412">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="77ea9-412">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="77ea9-413">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-413">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="77ea9-414">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-414">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="77ea9-415">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="77ea9-415">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-416">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-416">Profile</span></span>

* <span data-ttu-id="77ea9-417">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-417">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="77ea9-418">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="77ea9-418">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="77ea9-419">SGBDR</span><span class="sxs-lookup"><span data-stu-id="77ea9-419">RDBMS</span></span>

* <span data-ttu-id="77ea9-420">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="77ea9-420">Added `georestore` command</span></span>
* <span data-ttu-id="77ea9-421">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-421">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-422">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-422">Resource</span></span>

* <span data-ttu-id="77ea9-423">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-423">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="77ea9-424">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-424">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-425">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-425">SQL</span></span>

* <span data-ttu-id="77ea9-426">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="77ea9-426">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-427">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-427">Storage</span></span>

* <span data-ttu-id="77ea9-428">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="77ea9-428">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-429">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-429">VM</span></span>

* <span data-ttu-id="77ea9-430">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-430">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="77ea9-431">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="77ea9-431">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="77ea9-433">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-433">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="77ea9-434">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="77ea9-434">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="77ea9-435">#5718</span><span class="sxs-lookup"><span data-stu-id="77ea9-435">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="77ea9-436">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="77ea9-436">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="77ea9-437">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-437">March 27, 2018</span></span>

<span data-ttu-id="77ea9-438">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="77ea9-438">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-439">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-439">Core</span></span>

* <span data-ttu-id="77ea9-440">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="77ea9-440">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-441">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-441">ACS</span></span>

* <span data-ttu-id="77ea9-442">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="77ea9-442">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-443">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-443">Appservice</span></span>

* <span data-ttu-id="77ea9-444">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-444">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="77ea9-445">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-445">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="77ea9-446">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="77ea9-446">Backup</span></span>

* <span data-ttu-id="77ea9-447">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="77ea9-447">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="77ea9-448">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="77ea9-448">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="77ea9-449">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="77ea9-449">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="77ea9-450">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-450">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-451">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-451">Container</span></span>

* <span data-ttu-id="77ea9-452">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="77ea9-452">Added `container exec` command.</span></span> <span data-ttu-id="77ea9-453">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="77ea9-453">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="77ea9-454">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-454">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-455">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-455">Extension</span></span>

* <span data-ttu-id="77ea9-456">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="77ea9-456">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="77ea9-457">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="77ea9-457">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="77ea9-458">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-458">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-459">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-459">Interactive</span></span>

* <span data-ttu-id="77ea9-460">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-460">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="77ea9-461">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="77ea9-461">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="77ea9-462">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="77ea9-462">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="77ea9-463">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="77ea9-463">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="77ea9-464">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-464">Lab</span></span>

* <span data-ttu-id="77ea9-465">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="77ea9-465">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-466">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-466">Monitor</span></span>

* <span data-ttu-id="77ea9-467">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="77ea9-467">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="77ea9-468">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="77ea9-468">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="77ea9-469">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="77ea9-469">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-470">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-470">Network</span></span>

* <span data-ttu-id="77ea9-471">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="77ea9-471">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-472">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-472">Profile</span></span>

* <span data-ttu-id="77ea9-473">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="77ea9-473">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="77ea9-474">SGBDR</span><span class="sxs-lookup"><span data-stu-id="77ea9-474">RDBMS</span></span>

* <span data-ttu-id="77ea9-475">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="77ea9-475">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-476">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-476">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="77ea9-478">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-478">Role</span></span>

* <span data-ttu-id="77ea9-479">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-479">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="77ea9-480">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="77ea9-480">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="77ea9-481">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-481">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="77ea9-482">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-482">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="77ea9-483">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="77ea9-483">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-484">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-484">Storage</span></span>

* <span data-ttu-id="77ea9-485">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="77ea9-485">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="77ea9-486">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="77ea9-486">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-487">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-487">VM</span></span>

* <span data-ttu-id="77ea9-488">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="77ea9-488">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="77ea9-489">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-489">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="77ea9-490">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="77ea9-490">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="77ea9-491">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="77ea9-491">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="77ea9-492">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-492">March 13, 2018</span></span>

<span data-ttu-id="77ea9-493">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="77ea9-493">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-494">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-494">ACR</span></span>

* <span data-ttu-id="77ea9-495">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="77ea9-495">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="77ea9-496">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="77ea9-496">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="77ea9-497">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="77ea9-497">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-498">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-498">ACS</span></span>

* <span data-ttu-id="77ea9-499">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="77ea9-499">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="77ea9-500">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="77ea9-500">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="77ea9-501">Advisor</span><span class="sxs-lookup"><span data-stu-id="77ea9-501">Advisor</span></span>

* <span data-ttu-id="77ea9-502">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-502">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="77ea9-503">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-503">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="77ea9-504">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="77ea9-504">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="77ea9-505">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-505">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="77ea9-506">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-506">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-507">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-507">Appservice</span></span>

* <span data-ttu-id="77ea9-508">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="77ea9-508">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="77ea9-509">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-509">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="77ea9-510">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="77ea9-510">Eventhubs</span></span>

* <span data-ttu-id="77ea9-511">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-511">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-512">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-512">Extension</span></span>

* <span data-ttu-id="77ea9-513">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-513">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-514">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-514">Interactive</span></span>

* <span data-ttu-id="77ea9-515">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="77ea9-515">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="77ea9-516">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="77ea9-516">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="77ea9-517">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="77ea9-517">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="77ea9-518">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="77ea9-518">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-519">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-519">Monitor</span></span>

* <span data-ttu-id="77ea9-520">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="77ea9-520">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="77ea9-521">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="77ea9-521">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="77ea9-522">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="77ea9-522">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="77ea9-523">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="77ea9-523">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-524">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-524">Network</span></span>

* <span data-ttu-id="77ea9-525">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-525">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="77ea9-526">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="77ea9-526">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="77ea9-527">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="77ea9-527">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="77ea9-528">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="77ea9-528">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-529">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-529">Profile</span></span>

* <span data-ttu-id="77ea9-530">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="77ea9-530">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="77ea9-531">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="77ea9-531">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="77ea9-532">SGBDR</span><span class="sxs-lookup"><span data-stu-id="77ea9-532">RDBMS</span></span>

* <span data-ttu-id="77ea9-533">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="77ea9-533">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="77ea9-534">Service Bus</span><span class="sxs-lookup"><span data-stu-id="77ea9-534">Service Bus</span></span>

* <span data-ttu-id="77ea9-535">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-535">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-536">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-536">Storage</span></span>

* <span data-ttu-id="77ea9-537">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="77ea9-537">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="77ea9-538">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="77ea9-538">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-539">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-539">VM</span></span>

* <span data-ttu-id="77ea9-540">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="77ea9-540">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="77ea9-541">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="77ea9-541">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="77ea9-542">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="77ea9-542">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="77ea9-543">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="77ea9-543">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="77ea9-544">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-544">February 27, 2018</span></span>

<span data-ttu-id="77ea9-545">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="77ea9-545">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-546">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-546">Core</span></span>

* <span data-ttu-id="77ea9-547">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="77ea9-547">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="77ea9-548">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="77ea9-548">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="77ea9-549">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="77ea9-549">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-550">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-550">ACS</span></span>

* <span data-ttu-id="77ea9-551">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-551">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="77ea9-552">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="77ea9-552">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="77ea9-553">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="77ea9-553">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="77ea9-554">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="77ea9-554">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-555">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-555">Appservice</span></span>

* <span data-ttu-id="77ea9-556">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="77ea9-556">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="77ea9-557">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="77ea9-557">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="77ea9-558">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="77ea9-558">Cognitive Services</span></span>

* <span data-ttu-id="77ea9-559">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="77ea9-559">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="77ea9-560">Consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-560">Consumption</span></span>

* <span data-ttu-id="77ea9-561">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="77ea9-561">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="77ea9-562">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="77ea9-562">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-563">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-563">Container</span></span>

* <span data-ttu-id="77ea9-564">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="77ea9-564">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-565">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-565">Network</span></span>

* <span data-ttu-id="77ea9-566">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="77ea9-566">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-567">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-567">Resource</span></span>

* <span data-ttu-id="77ea9-568">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="77ea9-568">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-569">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-569">Role</span></span>

* <span data-ttu-id="77ea9-570">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="77ea9-570">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-571">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-571">SQL</span></span>

* <span data-ttu-id="77ea9-572">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="77ea9-572">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-573">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-573">Storage</span></span>

* <span data-ttu-id="77ea9-574">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-574">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-575">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-575">VM</span></span>

* <span data-ttu-id="77ea9-576">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="77ea9-576">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="77ea9-577">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-577">February 13, 2018</span></span>

<span data-ttu-id="77ea9-578">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="77ea9-578">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-579">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-579">Core</span></span>

* <span data-ttu-id="77ea9-580">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="77ea9-580">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-581">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-581">ACS</span></span>

* <span data-ttu-id="77ea9-582">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="77ea9-582">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="77ea9-583">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-583">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="77ea9-584">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="77ea9-584">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="77ea9-585">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="77ea9-585">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="77ea9-586">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="77ea9-586">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="77ea9-587">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="77ea9-587">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="77ea9-588">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="77ea9-588">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="77ea9-589">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="77ea9-589">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-590">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-590">Appservice</span></span>

* <span data-ttu-id="77ea9-591">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="77ea9-591">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="77ea9-592">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="77ea9-592">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="77ea9-593">CDN</span><span class="sxs-lookup"><span data-stu-id="77ea9-593">CDN</span></span>

* <span data-ttu-id="77ea9-594">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-594">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-595">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-595">Container</span></span>

* <span data-ttu-id="77ea9-596">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="77ea9-596">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="77ea9-597">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-597">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77ea9-598">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77ea9-598">CosmosDB</span></span>

* <span data-ttu-id="77ea9-599">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="77ea9-599">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-600">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-600">Extension</span></span>

* <span data-ttu-id="77ea9-601">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-601">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="77ea9-602">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-602">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="77ea9-603">Commentaires</span><span class="sxs-lookup"><span data-stu-id="77ea9-603">Feedback</span></span>

* <span data-ttu-id="77ea9-604">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="77ea9-604">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-605">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-605">Interactive</span></span>

* <span data-ttu-id="77ea9-606">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="77ea9-606">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="77ea9-607">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="77ea9-607">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-608">IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-608">IoT</span></span>

* <span data-ttu-id="77ea9-609">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="77ea9-609">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="77ea9-610">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="77ea9-610">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="77ea9-611">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-611">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="77ea9-612">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="77ea9-612">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-613">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-613">Monitor</span></span>

* <span data-ttu-id="77ea9-614">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-614">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-615">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-615">Network</span></span>

* <span data-ttu-id="77ea9-616">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="77ea9-616">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="77ea9-617">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-617">Profile</span></span>

* <span data-ttu-id="77ea9-618">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="77ea9-618">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-619">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-619">Resource</span></span>

* <span data-ttu-id="77ea9-620">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-620">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-621">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-621">Role</span></span>

* <span data-ttu-id="77ea9-622">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-622">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-623">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-623">SQL</span></span>

* <span data-ttu-id="77ea9-624">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="77ea9-624">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="77ea9-625">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="77ea9-625">Added `sql db rename`</span></span>
* <span data-ttu-id="77ea9-626">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="77ea9-626">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-627">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-627">Storage</span></span>

* <span data-ttu-id="77ea9-628">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="77ea9-628">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-629">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-629">VM</span></span>

* <span data-ttu-id="77ea9-630">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="77ea9-630">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="77ea9-631">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="77ea9-631">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="77ea9-632">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="77ea9-632">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="77ea9-633">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-633">January 31, 2018</span></span>

<span data-ttu-id="77ea9-634">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="77ea9-634">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-635">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-635">Core</span></span>

* <span data-ttu-id="77ea9-636">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="77ea9-636">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="77ea9-637">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="77ea9-637">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="77ea9-638">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="77ea9-638">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="77ea9-639">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="77ea9-639">Use `--verbose` to see</span></span>
* <span data-ttu-id="77ea9-640">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="77ea9-640">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-641">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-641">ACS</span></span>

* <span data-ttu-id="77ea9-642">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="77ea9-642">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="77ea9-643">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="77ea9-643">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-644">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-644">Appservice</span></span>

* <span data-ttu-id="77ea9-645">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="77ea9-645">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="77ea9-646">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="77ea9-646">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="77ea9-647">CDN</span><span class="sxs-lookup"><span data-stu-id="77ea9-647">CDN</span></span>

* <span data-ttu-id="77ea9-648">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-648">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77ea9-649">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77ea9-649">CosmosDB</span></span>

* <span data-ttu-id="77ea9-650">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="77ea9-650">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-651">Interactive</span></span>

* <span data-ttu-id="77ea9-652">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="77ea9-652">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-653">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-653">Network</span></span>

* <span data-ttu-id="77ea9-654">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-654">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="77ea9-655">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-655">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="77ea9-656">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-656">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="77ea9-657">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-657">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="77ea9-658">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="77ea9-658">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="77ea9-659">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="77ea9-659">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="77ea9-660">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="77ea9-660">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="77ea9-661">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="77ea9-661">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="77ea9-662">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="77ea9-662">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="77ea9-663">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="77ea9-663">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-664">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-664">Profile</span></span>

* <span data-ttu-id="77ea9-665">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="77ea9-665">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-666">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-666">Resource</span></span>

* <span data-ttu-id="77ea9-667">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="77ea9-667">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-668">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-668">Storage</span></span>

* <span data-ttu-id="77ea9-669">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="77ea9-669">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="77ea9-670">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="77ea9-670">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="77ea9-671">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-671">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="77ea9-672">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-672">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="77ea9-673">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="77ea9-673">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-674">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-674">VM</span></span>

* <span data-ttu-id="77ea9-675">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="77ea9-675">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="77ea9-676">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="77ea9-676">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="77ea9-677">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="77ea9-677">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="77ea9-678">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-678">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="77ea9-679">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="77ea9-679">January 17, 2018</span></span>

<span data-ttu-id="77ea9-680">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="77ea9-680">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-681">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-681">ACR</span></span>

* <span data-ttu-id="77ea9-682">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="77ea9-682">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="77ea9-683">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="77ea9-683">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-684">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-684">ACS</span></span>

* <span data-ttu-id="77ea9-685">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="77ea9-685">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="77ea9-686">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="77ea9-686">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-687">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-687">Appservice</span></span>

* <span data-ttu-id="77ea9-688">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="77ea9-688">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="77ea9-689">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="77ea9-689">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="77ea9-690">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="77ea9-690">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="77ea9-691">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="77ea9-691">Backup</span></span>

* <span data-ttu-id="77ea9-692">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="77ea9-692">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="77ea9-693">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="77ea9-693">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="77ea9-694">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="77ea9-694">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="77ea9-695">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="77ea9-695">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="77ea9-696">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-696">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-697">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-697">Batch</span></span>

* <span data-ttu-id="77ea9-698">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="77ea9-698">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="77ea9-699">Cloud</span><span class="sxs-lookup"><span data-stu-id="77ea9-699">Cloud</span></span>

* <span data-ttu-id="77ea9-700">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="77ea9-700">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="77ea9-701">Consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-701">Consumption</span></span>

* <span data-ttu-id="77ea9-702">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="77ea9-702">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="77ea9-703">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77ea9-703">Event Grid</span></span>

* <span data-ttu-id="77ea9-704">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="77ea9-704">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="77ea9-705">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="77ea9-705">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="77ea9-706">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="77ea9-706">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="77ea9-707">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="77ea9-707">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="77ea9-708">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-708">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="77ea9-709">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-709">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="77ea9-710">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="77ea9-710">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="77ea9-711">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="77ea9-711">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-712">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-712">Interactive</span></span>

* <span data-ttu-id="77ea9-713">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="77ea9-713">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="77ea9-714">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="77ea9-714">Fixed errors on startup</span></span>
* <span data-ttu-id="77ea9-715">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="77ea9-715">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-716">IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-716">IoT</span></span>

* <span data-ttu-id="77ea9-717">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="77ea9-717">Added support for device provisioning service</span></span>
* <span data-ttu-id="77ea9-718">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-718">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="77ea9-719">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-719">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-720">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-720">Monitor</span></span>

* <span data-ttu-id="77ea9-721">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="77ea9-721">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="77ea9-722">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-722">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="77ea9-723">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="77ea9-723">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-724">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-724">Network</span></span>

* <span data-ttu-id="77ea9-725">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-725">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="77ea9-726">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-726">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-727">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-727">Profile</span></span>

* <span data-ttu-id="77ea9-728">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-728">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-729">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-729">Role</span></span>

* <span data-ttu-id="77ea9-730">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="77ea9-730">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77ea9-731">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77ea9-731">Service Fabric</span></span>

* <span data-ttu-id="77ea9-732">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="77ea9-732">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="77ea9-733">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-733">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-734">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-734">VM</span></span>

* <span data-ttu-id="77ea9-735">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="77ea9-735">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="77ea9-736">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="77ea9-736">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="77ea9-737">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="77ea9-737">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="77ea9-738">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="77ea9-738">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="77ea9-739">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="77ea9-739">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="77ea9-740">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-740">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="77ea9-741">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-741">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="77ea9-742">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="77ea9-742">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="77ea9-743">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-743">December 19, 2017</span></span>

<span data-ttu-id="77ea9-744">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="77ea9-744">Version 2.0.23</span></span>

* <span data-ttu-id="77ea9-745">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-745">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-746">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-746">Container</span></span>

* <span data-ttu-id="77ea9-747">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-747">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-748">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-748">Network</span></span>

* <span data-ttu-id="77ea9-749">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-749">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="77ea9-750">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-750">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-751">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-751">Storage</span></span>

* <span data-ttu-id="77ea9-752">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="77ea9-752">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-753">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-753">VM</span></span>

* <span data-ttu-id="77ea9-754">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="77ea9-754">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="77ea9-755">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-755">December 5, 2017</span></span>

<span data-ttu-id="77ea9-756">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="77ea9-756">Version 2.0.22</span></span>

* <span data-ttu-id="77ea9-757">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-757">Removed `az component` commands.</span></span> <span data-ttu-id="77ea9-758">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="77ea9-758">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-759">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-759">Core</span></span>
* <span data-ttu-id="77ea9-760">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="77ea9-760">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="77ea9-761">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="77ea9-761">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-762">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-762">ACS</span></span>

* <span data-ttu-id="77ea9-763">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="77ea9-763">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="77ea9-764">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-764">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="77ea9-765">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="77ea9-765">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="77ea9-766">Advisor</span><span class="sxs-lookup"><span data-stu-id="77ea9-766">Advisor</span></span>

* <span data-ttu-id="77ea9-767">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-767">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-768">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-768">Appservice</span></span>

* <span data-ttu-id="77ea9-769">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="77ea9-769">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="77ea9-770">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="77ea9-770">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="77ea9-771">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="77ea9-771">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="77ea9-772">Consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-772">Consumption</span></span>

* <span data-ttu-id="77ea9-773">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="77ea9-773">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-774">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-774">Container</span></span>

* <span data-ttu-id="77ea9-775">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-775">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-776">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-776">Monitor</span></span>

* <span data-ttu-id="77ea9-777">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="77ea9-777">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-778">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-778">Resource</span></span>

* <span data-ttu-id="77ea9-779">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-779">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-780">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-780">Role</span></span>

* <span data-ttu-id="77ea9-781">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-781">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="77ea9-782">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="77ea9-782">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="77ea9-783">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="77ea9-783">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-784">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-784">SQL</span></span>

* <span data-ttu-id="77ea9-785">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="77ea9-785">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="77ea9-786">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-786">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-787">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-787">VM</span></span>

* <span data-ttu-id="77ea9-788">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="77ea9-788">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="77ea9-789">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-789">November 14, 2017</span></span>

<span data-ttu-id="77ea9-790">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="77ea9-790">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-791">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-791">ACR</span></span>

* <span data-ttu-id="77ea9-792">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="77ea9-792">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="77ea9-793">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-793">ACS</span></span>

* <span data-ttu-id="77ea9-794">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="77ea9-794">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="77ea9-795">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-795">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="77ea9-796">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="77ea9-796">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="77ea9-797">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="77ea9-797">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="77ea9-798">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="77ea9-798">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-799">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-799">Appservice</span></span>

* <span data-ttu-id="77ea9-800">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="77ea9-800">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="77ea9-801">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="77ea9-801">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="77ea9-802">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="77ea9-802">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="77ea9-803">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="77ea9-803">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="77ea9-804">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="77ea9-804">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="77ea9-805">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="77ea9-805">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-806">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-806">Batch</span></span>

* <span data-ttu-id="77ea9-807">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="77ea9-807">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="77ea9-808">Batchai</span><span class="sxs-lookup"><span data-stu-id="77ea9-808">Batchai</span></span>

* <span data-ttu-id="77ea9-809">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-809">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="77ea9-810">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-810">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="77ea9-811">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="77ea9-811">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="77ea9-812">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-812">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="77ea9-813">Cloud</span><span class="sxs-lookup"><span data-stu-id="77ea9-813">Cloud</span></span>

* <span data-ttu-id="77ea9-814">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="77ea9-814">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-815">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-815">Container</span></span>

* <span data-ttu-id="77ea9-816">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="77ea9-816">Added support to open multiple ports</span></span>
* <span data-ttu-id="77ea9-817">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="77ea9-817">Added container group restart policy</span></span>
* <span data-ttu-id="77ea9-818">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="77ea9-818">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="77ea9-819">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="77ea9-819">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77ea9-820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77ea9-820">Data Lake Analytics</span></span>

* <span data-ttu-id="77ea9-821">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="77ea9-821">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77ea9-822">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-822">Data Lake Store</span></span>

* <span data-ttu-id="77ea9-823">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="77ea9-823">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-824">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-824">Extension</span></span>

* <span data-ttu-id="77ea9-825">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="77ea9-825">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="77ea9-826">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="77ea9-826">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-827">IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-827">IoT</span></span>

* <span data-ttu-id="77ea9-828">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="77ea9-828">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-829">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-829">Monitor</span></span>

* <span data-ttu-id="77ea9-830">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="77ea9-830">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-831">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-831">Network</span></span>

* <span data-ttu-id="77ea9-832">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="77ea9-832">Added support for CAA DNS records</span></span>
* <span data-ttu-id="77ea9-833">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-833">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="77ea9-834">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="77ea9-834">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="77ea9-835">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="77ea9-835">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="77ea9-836">Réservations</span><span class="sxs-lookup"><span data-stu-id="77ea9-836">Reservations</span></span>

* <span data-ttu-id="77ea9-837">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-837">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-838">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-838">Resource</span></span>

* <span data-ttu-id="77ea9-839">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="77ea9-839">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-840">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-840">SQL</span></span>

* <span data-ttu-id="77ea9-841">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-841">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-842">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-842">Storage</span></span>

* <span data-ttu-id="77ea9-843">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-843">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="77ea9-844">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="77ea9-844">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="77ea9-845">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="77ea9-845">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="77ea9-846">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="77ea9-846">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="77ea9-847">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-847">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="77ea9-848">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="77ea9-848">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="77ea9-849">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-849">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-850">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-850">VM</span></span>

* <span data-ttu-id="77ea9-851">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="77ea9-851">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="77ea9-852">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="77ea9-852">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="77ea9-853">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="77ea9-853">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="77ea9-854">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="77ea9-854">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="77ea9-855">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="77ea9-855">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="77ea9-856">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-856">October 24, 2017</span></span>

<span data-ttu-id="77ea9-857">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="77ea9-857">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-858">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-858">Core</span></span>

* <span data-ttu-id="77ea9-859">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="77ea9-859">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-860">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-860">ACR</span></span>

* <span data-ttu-id="77ea9-861">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="77ea9-861">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="77ea9-862">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="77ea9-862">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="77ea9-863">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="77ea9-863">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-864">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-864">ACS</span></span>

* <span data-ttu-id="77ea9-865">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="77ea9-865">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="77ea9-866">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="77ea9-866">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-867">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-867">Appservice</span></span>

* <span data-ttu-id="77ea9-868">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="77ea9-868">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="77ea9-869">Composant</span><span class="sxs-lookup"><span data-stu-id="77ea9-869">Component</span></span>

* <span data-ttu-id="77ea9-870">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="77ea9-870">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-871">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-871">Monitor</span></span>

* <span data-ttu-id="77ea9-872">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="77ea9-872">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-873">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-873">Resource</span></span>

* <span data-ttu-id="77ea9-874">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="77ea9-874">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="77ea9-875">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="77ea9-875">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-876">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-876">VM</span></span>

* <span data-ttu-id="77ea9-877">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-877">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="77ea9-878">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-878">October 9, 2017</span></span>

<span data-ttu-id="77ea9-879">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="77ea9-879">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-880">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-880">Core</span></span>

* <span data-ttu-id="77ea9-881">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="77ea9-881">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-882">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-882">Appservice</span></span>

* <span data-ttu-id="77ea9-883">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-883">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-884">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-884">Batch</span></span>

* <span data-ttu-id="77ea9-885">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="77ea9-885">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="77ea9-886">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="77ea9-886">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="77ea9-887">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-887">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="77ea9-888">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="77ea9-888">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="77ea9-889">Batchai</span><span class="sxs-lookup"><span data-stu-id="77ea9-889">Batchai</span></span>

* <span data-ttu-id="77ea9-890">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="77ea9-890">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-891">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-891">Keyvault</span></span>

* <span data-ttu-id="77ea9-892">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="77ea9-892">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="77ea9-893">(#4448)</span><span class="sxs-lookup"><span data-stu-id="77ea9-893">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="77ea9-894">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-894">Network</span></span>

* <span data-ttu-id="77ea9-895">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="77ea9-895">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="77ea9-896">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="77ea9-896">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-897">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-897">Resource</span></span>

* <span data-ttu-id="77ea9-898">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="77ea9-898">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="77ea9-899">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="77ea9-899">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="77ea9-900">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="77ea9-900">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="77ea9-901">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="77ea9-901">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-902">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-902">Sql</span></span>

* <span data-ttu-id="77ea9-903">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="77ea9-903">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="77ea9-904">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="77ea9-904">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="77ea9-905">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="77ea9-905">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-906">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-906">Storage</span></span>

* <span data-ttu-id="77ea9-907">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="77ea9-907">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-908">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-908">Vm</span></span>

* <span data-ttu-id="77ea9-909">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="77ea9-909">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="77ea9-910">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-910">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="77ea9-911">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="77ea9-911">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="77ea9-912">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-912">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="77ea9-913">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-913">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="77ea9-914">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-914">September 22, 2017</span></span>

<span data-ttu-id="77ea9-915">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="77ea9-915">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-916">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-916">Resource</span></span>

* <span data-ttu-id="77ea9-917">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="77ea9-917">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="77ea9-918">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="77ea9-918">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="77ea9-919">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-919">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="77ea9-920">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="77ea9-920">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-921">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-921">Network</span></span>

* <span data-ttu-id="77ea9-922">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="77ea9-922">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="77ea9-923">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="77ea9-923">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="77ea9-924">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="77ea9-924">Added `asg` application security group commands</span></span>
* <span data-ttu-id="77ea9-925">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-925">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="77ea9-926">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-926">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="77ea9-927">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-927">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="77ea9-928">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-928">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-929">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-929">Storage</span></span>

* <span data-ttu-id="77ea9-930">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77ea9-930">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="77ea9-931">Événement</span><span class="sxs-lookup"><span data-stu-id="77ea9-931">Eventgrid</span></span>

* <span data-ttu-id="77ea9-932">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="77ea9-932">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-933">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-933">SQL</span></span>

* <span data-ttu-id="77ea9-934">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="77ea9-934">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="77ea9-935">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="77ea9-935">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="77ea9-936">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-936">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-937">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-937">Keyvault</span></span>

* <span data-ttu-id="77ea9-938">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="77ea9-938">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-939">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-939">VM</span></span>

* <span data-ttu-id="77ea9-940">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-940">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="77ea9-941">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="77ea9-941">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="77ea9-942">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-942">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="77ea9-943">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="77ea9-943">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="77ea9-944">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="77ea9-944">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="77ea9-945">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="77ea9-945">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-946">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-946">ACS</span></span>

* <span data-ttu-id="77ea9-947">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="77ea9-947">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-948">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-948">Appservice</span></span>

* <span data-ttu-id="77ea9-949">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-949">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="77ea9-950">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="77ea9-950">Backup</span></span>

* <span data-ttu-id="77ea9-951">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="77ea9-951">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="77ea9-952">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-952">September 11, 2017</span></span>

<span data-ttu-id="77ea9-953">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="77ea9-953">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="77ea9-954">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-954">Core</span></span>

* <span data-ttu-id="77ea9-955">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="77ea9-955">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="77ea9-956">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="77ea9-956">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-957">Acs</span><span class="sxs-lookup"><span data-stu-id="77ea9-957">Acs</span></span>

* <span data-ttu-id="77ea9-958">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="77ea9-958">Added `acs list-locations` command</span></span>
* <span data-ttu-id="77ea9-959">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="77ea9-959">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-960">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-960">Appservice</span></span>

* <span data-ttu-id="77ea9-961">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="77ea9-961">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="77ea9-962">CDN</span><span class="sxs-lookup"><span data-stu-id="77ea9-962">CDN</span></span>

* <span data-ttu-id="77ea9-963">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-963">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="77ea9-964">Extension</span><span class="sxs-lookup"><span data-stu-id="77ea9-964">Extension</span></span>

* <span data-ttu-id="77ea9-965">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-965">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-966">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-966">Keyvault</span></span>

* <span data-ttu-id="77ea9-967">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="77ea9-967">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-968">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-968">Network</span></span>

* <span data-ttu-id="77ea9-969">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="77ea9-969">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="77ea9-970">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-970">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="77ea9-971">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-971">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="77ea9-972">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-972">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="77ea9-973">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-973">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-974">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-974">Resource</span></span>

* <span data-ttu-id="77ea9-975">Autoriser les passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-975">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="77ea9-976">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-976">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="77ea9-977">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="77ea9-977">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="77ea9-978">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="77ea9-978">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-979">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-979">SQL</span></span>

* <span data-ttu-id="77ea9-980">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="77ea9-980">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-981">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-981">VM</span></span>

* <span data-ttu-id="77ea9-982">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="77ea9-982">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="77ea9-983">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="77ea9-983">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="77ea9-984">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-984">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="77ea9-985">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="77ea9-985">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="77ea9-986">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="77ea9-986">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="77ea9-987">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-987">August 31, 2017</span></span>

<span data-ttu-id="77ea9-988">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="77ea9-988">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-989">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-989">Keyvault</span></span>

* <span data-ttu-id="77ea9-990">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="77ea9-990">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="77ea9-991">Sf</span><span class="sxs-lookup"><span data-stu-id="77ea9-991">Sf</span></span>

* <span data-ttu-id="77ea9-992">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="77ea9-992">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-993">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-993">Storage</span></span>

* <span data-ttu-id="77ea9-994">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="77ea9-994">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="77ea9-995">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="77ea9-995">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="77ea9-996">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-996">August 28, 2017</span></span>

<span data-ttu-id="77ea9-997">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="77ea9-997">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="77ea9-998">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-998">CLI</span></span>

* <span data-ttu-id="77ea9-999">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="77ea9-999">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1000">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1000">ACS</span></span>

* <span data-ttu-id="77ea9-1001">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="77ea9-1001">Corrected preview regions</span></span>
* <span data-ttu-id="77ea9-1002">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1002">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="77ea9-1003">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1003">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-1004">Appservice</span></span>

* <span data-ttu-id="77ea9-1005">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1005">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="77ea9-1006">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1006">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="77ea9-1007">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1007">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="77ea9-1008">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1008">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="77ea9-1009">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1009">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-1010">IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-1010">IoT</span></span>

* <span data-ttu-id="77ea9-1011">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="77ea9-1011">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-1012">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1012">Network</span></span>

* <span data-ttu-id="77ea9-1013">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1013">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="77ea9-1014">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1014">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="77ea9-1015">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1015">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="77ea9-1016">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1016">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="77ea9-1017">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1017">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-1018">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-1018">Profile</span></span>

* <span data-ttu-id="77ea9-1019">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1019">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77ea9-1020">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77ea9-1020">Service Fabric</span></span>

* <span data-ttu-id="77ea9-1021">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1021">Preview release</span></span>
* <span data-ttu-id="77ea9-1022">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-1022">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="77ea9-1023">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="77ea9-1023">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="77ea9-1024">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1024">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-1025">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1025">Storage</span></span>

* <span data-ttu-id="77ea9-1026">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="77ea9-1026">Enabled setting blob tier</span></span>
* <span data-ttu-id="77ea9-1027">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="77ea9-1027">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="77ea9-1028">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1028">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="77ea9-1029">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="77ea9-1029">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="77ea9-1030">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1030">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="77ea9-1031">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="77ea9-1031">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-1032">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1032">VM</span></span>

* <span data-ttu-id="77ea9-1033">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1033">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="77ea9-1034">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="77ea9-1034">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="77ea9-1035">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1035">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="77ea9-1036">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="77ea9-1036">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="77ea9-1037">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="77ea9-1037">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="77ea9-1038">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1038">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="77ea9-1039">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1039">August 15, 2017</span></span>

<span data-ttu-id="77ea9-1040">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="77ea9-1040">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1041">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1041">ACS</span></span>

* <span data-ttu-id="77ea9-1042">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="77ea9-1042">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-1043">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-1043">Appservice</span></span>

* <span data-ttu-id="77ea9-1044">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="77ea9-1044">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="77ea9-1045">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77ea9-1045">Event Grid</span></span>

* <span data-ttu-id="77ea9-1046">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1046">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="77ea9-1047">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1047">August 11, 2017</span></span>

<span data-ttu-id="77ea9-1048">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="77ea9-1048">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1049">ACS</span></span>

* <span data-ttu-id="77ea9-1050">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="77ea9-1050">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-1051">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-1051">Batch</span></span>

* <span data-ttu-id="77ea9-1052">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="77ea9-1052">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="77ea9-1053">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-1053">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="77ea9-1054">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="77ea9-1054">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="77ea9-1055">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="77ea9-1055">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="77ea9-1056">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="77ea9-1056">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="77ea9-1057">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="77ea9-1057">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="77ea9-1058">Composant</span><span class="sxs-lookup"><span data-stu-id="77ea9-1058">Component</span></span>

* <span data-ttu-id="77ea9-1059">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="77ea9-1059">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="77ea9-1060">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-1060">Container</span></span>

* <span data-ttu-id="77ea9-1061">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1061">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="77ea9-1062">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1062">Data Lake Store</span></span>

* <span data-ttu-id="77ea9-1063">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="77ea9-1063">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="77ea9-1064">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77ea9-1064">Event Grid</span></span>

* <span data-ttu-id="77ea9-1065">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77ea9-1065">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-1066">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1066">Network</span></span>

* <span data-ttu-id="77ea9-1067">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="77ea9-1067">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="77ea9-1068">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1068">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="77ea9-1069">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="77ea9-1069">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="77ea9-1070">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1070">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-1071">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-1071">Profile</span></span>

* <span data-ttu-id="77ea9-1072">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="77ea9-1072">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-1073">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1073">Storage</span></span>

* <span data-ttu-id="77ea9-1074">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="77ea9-1074">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-1075">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1075">VM</span></span>

* <span data-ttu-id="77ea9-1076">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="77ea9-1076">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="77ea9-1077">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1077">Exposed `list-skus` command</span></span>
* <span data-ttu-id="77ea9-1078">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1078">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="77ea9-1079">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="77ea9-1079">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="77ea9-1080">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="77ea9-1080">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="77ea9-1081">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1081">July 28, 2017</span></span>

<span data-ttu-id="77ea9-1082">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="77ea9-1082">Version 2.0.12</span></span>

* <span data-ttu-id="77ea9-1083">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="77ea9-1083">Added container commands</span></span>
* <span data-ttu-id="77ea9-1084">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="77ea9-1084">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="77ea9-1085">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-1085">Core</span></span>

* <span data-ttu-id="77ea9-1086">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="77ea9-1086">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="77ea9-1087">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1087">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="77ea9-1088">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1088">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="77ea9-1089">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1089">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="77ea9-1090">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="77ea9-1090">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="77ea9-1091">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1091">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="77ea9-1092">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1092">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77ea9-1093">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1093">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="77ea9-1094">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1094">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="77ea9-1095">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1095">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="77ea9-1096">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="77ea9-1096">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="77ea9-1097">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1097">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="77ea9-1098">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="77ea9-1098">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="77ea9-1099">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="77ea9-1099">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="77ea9-1100">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="77ea9-1100">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="77ea9-1101">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1101">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="77ea9-1102">ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-1102">ACR</span></span>

* <span data-ttu-id="77ea9-1103">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="77ea9-1103">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="77ea9-1104">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="77ea9-1104">Support SKU update for managed registries</span></span>
* <span data-ttu-id="77ea9-1105">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1105">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="77ea9-1106">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="77ea9-1106">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="77ea9-1107">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="77ea9-1107">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="77ea9-1108">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="77ea9-1108">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1109">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1109">ACS</span></span>

* <span data-ttu-id="77ea9-1110">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="77ea9-1110">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-1111">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-1111">Appservice</span></span>

* <span data-ttu-id="77ea9-1112">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="77ea9-1112">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="77ea9-1113">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="77ea9-1113">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="77ea9-1114">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1114">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="77ea9-1115">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1115">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="77ea9-1116">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1116">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="77ea9-1117">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1117">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="77ea9-1118">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1118">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="77ea9-1119">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1119">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="77ea9-1120">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1120">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="77ea9-1121">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1121">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="77ea9-1122">Batch</span><span class="sxs-lookup"><span data-stu-id="77ea9-1122">Batch</span></span>

* <span data-ttu-id="77ea9-1123">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="77ea9-1123">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="77ea9-1124">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1124">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="77ea9-1125">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1125">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="77ea9-1126">CDN</span><span class="sxs-lookup"><span data-stu-id="77ea9-1126">CDN</span></span>

* <span data-ttu-id="77ea9-1127">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="77ea9-1127">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="77ea9-1128">Cloud</span><span class="sxs-lookup"><span data-stu-id="77ea9-1128">Cloud</span></span>

* <span data-ttu-id="77ea9-1129">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="77ea9-1129">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="77ea9-1130">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1130">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="77ea9-1131">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="77ea9-1131">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="77ea9-1132">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="77ea9-1132">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="77ea9-1133">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1133">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77ea9-1134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77ea9-1134">CosmosDB</span></span>

* <span data-ttu-id="77ea9-1135">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1135">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="77ea9-1136">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="77ea9-1136">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77ea9-1137">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77ea9-1137">Data Lake Analytics</span></span>

* <span data-ttu-id="77ea9-1138">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1138">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="77ea9-1139">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1139">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="77ea9-1140">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1140">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77ea9-1141">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1141">Data Lake Store</span></span>

* <span data-ttu-id="77ea9-1142">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1142">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="77ea9-1143">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="77ea9-1143">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="77ea9-1144">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1144">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="77ea9-1145">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1145">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="77ea9-1146">Interactive</span><span class="sxs-lookup"><span data-stu-id="77ea9-1146">Interactive</span></span>

* <span data-ttu-id="77ea9-1147">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="77ea9-1147">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="77ea9-1148">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="77ea9-1148">Increased test coverage</span></span>
* <span data-ttu-id="77ea9-1149">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="77ea9-1149">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="77ea9-1150">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1150">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="77ea9-1151">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1151">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="77ea9-1152">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1152">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="77ea9-1153">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1153">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77ea9-1154">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1154">Added `--progress` flag</span></span>
* <span data-ttu-id="77ea9-1155">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="77ea9-1155">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="77ea9-1156">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1156">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="77ea9-1157">IoT</span><span class="sxs-lookup"><span data-stu-id="77ea9-1157">IoT</span></span>

* <span data-ttu-id="77ea9-1158">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1158">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="77ea9-1159">(#3934)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1159">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="77ea9-1160">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="77ea9-1160">Key vault</span></span>

* <span data-ttu-id="77ea9-1161">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1161">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="77ea9-1162">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1162">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="77ea9-1163">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1163">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77ea9-1164">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1164">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77ea9-1165">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1165">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="77ea9-1166">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1166">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="77ea9-1167">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1167">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="77ea9-1168">(#3307)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1168">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="77ea9-1169">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1169">Lab</span></span>

* <span data-ttu-id="77ea9-1170">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1170">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="77ea9-1171">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1171">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-1172">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-1172">Monitor</span></span>

* <span data-ttu-id="77ea9-1173">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1173">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="77ea9-1174">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1174">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="77ea9-1175">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1175">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="77ea9-1176">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1176">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="77ea9-1177">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1177">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="77ea9-1178">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="77ea9-1178">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="77ea9-1179">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="77ea9-1179">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="77ea9-1180">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1180">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="77ea9-1181">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1181">`location` no longer required</span></span>
  * <span data-ttu-id="77ea9-1182">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="77ea9-1182">Add name and ID support for target</span></span>
  * <span data-ttu-id="77ea9-1183">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1183">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="77ea9-1184">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1184">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="77ea9-1185">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="77ea9-1185">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="77ea9-1186">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="77ea9-1186">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="77ea9-1187">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1187">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="77ea9-1188">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1188">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-1189">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1189">Network</span></span>

* <span data-ttu-id="77ea9-1190">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1190">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="77ea9-1191">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1191">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="77ea9-1192">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="77ea9-1192">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="77ea9-1193">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="77ea9-1193">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="77ea9-1194">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1194">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="77ea9-1195">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1195">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="77ea9-1196">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1196">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="77ea9-1197">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1197">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="77ea9-1198">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1198">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="77ea9-1199">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1199">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="77ea9-1200">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1200">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="77ea9-1201">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1201">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="77ea9-1202">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1202">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="77ea9-1203">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1203">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="77ea9-1204">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1204">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="77ea9-1205">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1205">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="77ea9-1206">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1206">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="77ea9-1207">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1207">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="77ea9-1208">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1208">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="77ea9-1209">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1209">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="77ea9-1210">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1210">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="77ea9-1211">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-1211">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="77ea9-1212">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1212">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="77ea9-1213">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77ea9-1213">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="77ea9-1214">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77ea9-1214">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="77ea9-1215">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77ea9-1215">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="77ea9-1216">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77ea9-1216">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-1217">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-1217">Profile</span></span>

* <span data-ttu-id="77ea9-1218">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1218">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="77ea9-1219">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1219">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="77ea9-1220">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="77ea9-1220">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="77ea9-1221">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="77ea9-1221">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="77ea9-1222">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="77ea9-1222">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="77ea9-1223">SGBDR</span><span class="sxs-lookup"><span data-stu-id="77ea9-1223">RDBMS</span></span>

* <span data-ttu-id="77ea9-1224">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1224">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="77ea9-1225">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1225">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="77ea9-1226">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1226">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="77ea9-1227">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1227">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-1228">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-1228">Resource</span></span>

* <span data-ttu-id="77ea9-1229">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1229">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="77ea9-1230">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77ea9-1230">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="77ea9-1231">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77ea9-1231">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="77ea9-1232">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="77ea9-1232">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="77ea9-1233">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1233">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="77ea9-1234">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1234">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="77ea9-1235">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1235">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="77ea9-1236">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77ea9-1236">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-1237">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1237">Role</span></span>

* <span data-ttu-id="77ea9-1238">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1238">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="77ea9-1239">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1239">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="77ea9-1240">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="77ea9-1240">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="77ea9-1241">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1241">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="77ea9-1242">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1242">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77ea9-1243">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77ea9-1243">Service Fabric</span></span>
* <span data-ttu-id="77ea9-1244">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1244">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="77ea9-1245">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1245">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="77ea9-1246">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1246">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-1247">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-1247">SQL</span></span>

* <span data-ttu-id="77ea9-1248">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1248">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="77ea9-1249">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1249">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="77ea9-1250">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1250">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-1251">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1251">Storage</span></span>

* <span data-ttu-id="77ea9-1252">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1252">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="77ea9-1253">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="77ea9-1253">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="77ea9-1254">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1254">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="77ea9-1255">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1255">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="77ea9-1256">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1256">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="77ea9-1257">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1257">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-1258">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1258">VM</span></span>

* <span data-ttu-id="77ea9-1259">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1259">Support configuring nsg</span></span>
* <span data-ttu-id="77ea9-1260">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1260">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="77ea9-1261">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="77ea9-1261">Support managed service identities</span></span>
* <span data-ttu-id="77ea9-1262">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1262">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="77ea9-1263">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="77ea9-1263">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="77ea9-1264">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1264">May 10, 2017</span></span>

<span data-ttu-id="77ea9-1265">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="77ea9-1265">Version 2.0.6</span></span>

* <span data-ttu-id="77ea9-1266">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="77ea9-1266">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="77ea9-1267">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1267">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="77ea9-1268">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1268">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="77ea9-1269">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="77ea9-1269">Include Cognitive Services module</span></span>
* <span data-ttu-id="77ea9-1270">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77ea9-1270">Include Service Fabric module</span></span>
* <span data-ttu-id="77ea9-1271">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1271">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="77ea9-1272">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="77ea9-1272">Add support for CDN commands</span></span>
* <span data-ttu-id="77ea9-1273">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="77ea9-1273">Remove Container module</span></span>
* <span data-ttu-id="77ea9-1274">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1274">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="77ea9-1275">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1275">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="77ea9-1276">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-1276">Core</span></span>

* <span data-ttu-id="77ea9-1277">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1277">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="77ea9-1278">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1278">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="77ea9-1279">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1279">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="77ea9-1280">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1280">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="77ea9-1281">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1281">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="77ea9-1282">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1282">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="77ea9-1283">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1283">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="77ea9-1284">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1284">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="77ea9-1285">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1285">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="77ea9-1286">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="77ea9-1286">core: Improved performance</span></span>
* <span data-ttu-id="77ea9-1287">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="77ea9-1287">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="77ea9-1288">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="77ea9-1288">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1289">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1289">ACS</span></span>

* <span data-ttu-id="77ea9-1290">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="77ea9-1290">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="77ea9-1291">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="77ea9-1291">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="77ea9-1292">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="77ea9-1292">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="77ea9-1293">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1293">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-1294">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-1294">AppService</span></span>

* <span data-ttu-id="77ea9-1295">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1295">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="77ea9-1296">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="77ea9-1296">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="77ea9-1297">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1297">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="77ea9-1298">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="77ea9-1298">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="77ea9-1299">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="77ea9-1299">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="77ea9-1300">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1300">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="77ea9-1301">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="77ea9-1301">support slot swap with preview</span></span>
* <span data-ttu-id="77ea9-1302">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1302">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="77ea9-1303">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1303">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77ea9-1304">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77ea9-1304">CosmosDB</span></span>

* <span data-ttu-id="77ea9-1305">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="77ea9-1305">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="77ea9-1306">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="77ea9-1306">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="77ea9-1307">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="77ea9-1307">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="77ea9-1308">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="77ea9-1308">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77ea9-1309">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77ea9-1309">Data Lake Analytics</span></span>

* <span data-ttu-id="77ea9-1310">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="77ea9-1310">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="77ea9-1311">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1311">Add support for new catalog item type: package.</span></span> <span data-ttu-id="77ea9-1312">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1312">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="77ea9-1313">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1313">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="77ea9-1314">Table</span><span class="sxs-lookup"><span data-stu-id="77ea9-1314">Table</span></span>
  * <span data-ttu-id="77ea9-1315">Fonction table</span><span class="sxs-lookup"><span data-stu-id="77ea9-1315">Table valued function</span></span>
  * <span data-ttu-id="77ea9-1316">Affichage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1316">View</span></span>
  * <span data-ttu-id="77ea9-1317">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1317">Table Statistics.</span></span> <span data-ttu-id="77ea9-1318">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="77ea9-1318">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77ea9-1319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1319">Data Lake Store</span></span>

* <span data-ttu-id="77ea9-1320">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="77ea9-1320">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="77ea9-1321">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1321">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="77ea9-1322">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1322">missed help for access show.</span></span> <span data-ttu-id="77ea9-1323">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1323">adding it.</span></span> <span data-ttu-id="77ea9-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="77ea9-1325">Rechercher</span><span class="sxs-lookup"><span data-stu-id="77ea9-1325">Find</span></span>

* <span data-ttu-id="77ea9-1326">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="77ea9-1326">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="77ea9-1327">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77ea9-1327">KeyVault</span></span>

* <span data-ttu-id="77ea9-1328">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="77ea9-1328">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="77ea9-1329">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="77ea9-1329">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="77ea9-1330">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="77ea9-1330">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="77ea9-1331">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="77ea9-1331">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="77ea9-1332">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1332">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="77ea9-1333">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1333">Lab</span></span>

* <span data-ttu-id="77ea9-1334">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1334">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="77ea9-1335">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1335">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="77ea9-1336">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1336">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="77ea9-1337">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1337">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="77ea9-1338">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="77ea9-1338">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="77ea9-1339">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77ea9-1339">Monitor</span></span>

* <span data-ttu-id="77ea9-1340">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1340">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="77ea9-1341">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1341">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="77ea9-1342">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1342">Network</span></span>

* <span data-ttu-id="77ea9-1343">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1343">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="77ea9-1344">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1344">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="77ea9-1345">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="77ea9-1345">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="77ea9-1346">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="77ea9-1346">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="77ea9-1347">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="77ea9-1347">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="77ea9-1348">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="77ea9-1348">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="77ea9-1349">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="77ea9-1349">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="77ea9-1350">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="77ea9-1350">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="77ea9-1351">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1351">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="77ea9-1352">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="77ea9-1352">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="77ea9-1353">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1353">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="77ea9-1354">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1354">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="77ea9-1355">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1355">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="77ea9-1356">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="77ea9-1356">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="77ea9-1357">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="77ea9-1357">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="77ea9-1358">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="77ea9-1358">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="77ea9-1359">Profil</span><span class="sxs-lookup"><span data-stu-id="77ea9-1359">Profile</span></span>

* <span data-ttu-id="77ea9-1360">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1360">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="77ea9-1361">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1361">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="77ea9-1362">Redis</span><span class="sxs-lookup"><span data-stu-id="77ea9-1362">Redis</span></span>

* <span data-ttu-id="77ea9-1363">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="77ea9-1363">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="77ea9-1364">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="77ea9-1364">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="77ea9-1365">Ressource</span><span class="sxs-lookup"><span data-stu-id="77ea9-1365">Resource</span></span>

* <span data-ttu-id="77ea9-1366">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1366">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="77ea9-1367">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1367">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="77ea9-1368">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1368">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="77ea9-1369">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1369">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="77ea9-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="77ea9-1371">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1371">Add docs for az lock update.</span></span> <span data-ttu-id="77ea9-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="77ea9-1373">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1373">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="77ea9-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="77ea9-1375">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1375">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="77ea9-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="77ea9-1377">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1377">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="77ea9-1378">Rôle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1378">Role</span></span>

* <span data-ttu-id="77ea9-1379">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1379">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="77ea9-1380">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1380">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="77ea9-1381">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1381">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="77ea9-1382">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="77ea9-1382">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="77ea9-1383">SQL</span><span class="sxs-lookup"><span data-stu-id="77ea9-1383">SQL</span></span>

* <span data-ttu-id="77ea9-1384">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="77ea9-1384">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="77ea9-1385">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1385">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="77ea9-1386">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1386">Storage</span></span>

* <span data-ttu-id="77ea9-1387">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="77ea9-1387">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="77ea9-1388">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="77ea9-1388">Add support for incremental blob copy</span></span>
* <span data-ttu-id="77ea9-1389">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="77ea9-1389">Add support for large block blob upload</span></span>
* <span data-ttu-id="77ea9-1390">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="77ea9-1390">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-1391">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1391">VM</span></span>

* <span data-ttu-id="77ea9-1392">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="77ea9-1392">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="77ea9-1393">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1393">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="77ea9-1394">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="77ea9-1394">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="77ea9-1395">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="77ea9-1395">az vm/vmss disk</span></span>
  3. <span data-ttu-id="77ea9-1396">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="77ea9-1396">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="77ea9-1397">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="77ea9-1397">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="77ea9-1398">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1398">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="77ea9-1399">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1399">April 3, 2017</span></span>

<span data-ttu-id="77ea9-1400">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="77ea9-1400">Version 2.0.2</span></span>

<span data-ttu-id="77ea9-1401">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="77ea9-1401">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="77ea9-1402">Principal</span><span class="sxs-lookup"><span data-stu-id="77ea9-1402">Core</span></span>

* <span data-ttu-id="77ea9-1403">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-1403">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="77ea9-1404">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1404">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="77ea9-1405">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1405">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="77ea9-1406">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1406">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77ea9-1407">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1407">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="77ea9-1408">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1408">Add prompting for missing template parameters.</span></span> <span data-ttu-id="77ea9-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="77ea9-1410">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="77ea9-1410">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="77ea9-1411">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="77ea9-1411">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="77ea9-1412">ACS</span><span class="sxs-lookup"><span data-stu-id="77ea9-1412">ACS</span></span>

* <span data-ttu-id="77ea9-1413">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1413">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="77ea9-1414">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1414">Add support for ssh key password prompting.</span></span> <span data-ttu-id="77ea9-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="77ea9-1416">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1416">Add support for windows clusters.</span></span> <span data-ttu-id="77ea9-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="77ea9-1418">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1418">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="77ea9-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="77ea9-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="77ea9-1420">AppService</span></span>

* <span data-ttu-id="77ea9-1421">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1421">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="77ea9-1422">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1422">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="77ea9-1423">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1423">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="77ea9-1424">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1424">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="77ea9-1425">DataLake</span><span class="sxs-lookup"><span data-stu-id="77ea9-1425">DataLake</span></span>

* <span data-ttu-id="77ea9-1426">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77ea9-1426">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="77ea9-1427">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77ea9-1427">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="77ea9-1428">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="77ea9-1428">DocuemntDB</span></span>

* <span data-ttu-id="77ea9-1429">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1429">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="77ea9-1430">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77ea9-1430">VM</span></span>

* <span data-ttu-id="77ea9-1431">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1431">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="77ea9-1432">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1432">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="77ea9-1433">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1433">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="77ea9-1434">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1434">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77ea9-1435">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1435">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="77ea9-1436">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1436">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="77ea9-1437">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="77ea9-1437">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="77ea9-1438">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="77ea9-1438">February 27, 2017</span></span>

<span data-ttu-id="77ea9-1439">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="77ea9-1439">Version 2.0.0</span></span>

<span data-ttu-id="77ea9-1440">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1440">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="77ea9-1441">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1441">Container Service (acs)</span></span>
- <span data-ttu-id="77ea9-1442">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1442">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="77ea9-1443">Réseau</span><span class="sxs-lookup"><span data-stu-id="77ea9-1443">Networking</span></span>
- <span data-ttu-id="77ea9-1444">Stockage</span><span class="sxs-lookup"><span data-stu-id="77ea9-1444">Storage</span></span>

<span data-ttu-id="77ea9-1445">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1445">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="77ea9-1446">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1446">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="77ea9-1447">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1447">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="77ea9-1448">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1448">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="77ea9-1449">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="77ea9-1449">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="77ea9-1450">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="77ea9-1450">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="77ea9-1451">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="77ea9-1451">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="77ea9-1452">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="77ea9-1452">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="77ea9-1453">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="77ea9-1453">Provide feedback from the command line with the `az feedback` command</span></span>

