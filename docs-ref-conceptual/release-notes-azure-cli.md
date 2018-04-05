---
title: Notes de publication d’Azure CLI 2.0
description: En savoir plus sur les dernières mises à jour d’Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="efdb6-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="efdb6-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="efdb6-104">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-104">March 27, 2018</span></span>

<span data-ttu-id="efdb6-105">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="efdb6-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-106">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-106">Core</span></span>

* <span data-ttu-id="efdb6-107">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="efdb6-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-108">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-108">ACS</span></span>

* <span data-ttu-id="efdb6-109">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="efdb6-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-110">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-110">Appservice</span></span>

* <span data-ttu-id="efdb6-111">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="efdb6-112">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="efdb6-113">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="efdb6-113">Backup</span></span>

* <span data-ttu-id="efdb6-114">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="efdb6-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="efdb6-115">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="efdb6-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="efdb6-116">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="efdb6-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="efdb6-117">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-118">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-118">Container</span></span>

* <span data-ttu-id="efdb6-119">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="efdb6-119">Added `container exec` command.</span></span> <span data-ttu-id="efdb6-120">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="efdb6-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="efdb6-121">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="efdb6-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="efdb6-122">Extension</span><span class="sxs-lookup"><span data-stu-id="efdb6-122">Extension</span></span>

* <span data-ttu-id="efdb6-123">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="efdb6-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="efdb6-124">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="efdb6-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="efdb6-125">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-126">Interactive</span></span>

* <span data-ttu-id="efdb6-127">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="efdb6-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="efdb6-128">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="efdb6-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="efdb6-129">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="efdb6-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="efdb6-130">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="efdb6-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="efdb6-131">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-131">Lab</span></span>

* <span data-ttu-id="efdb6-132">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="efdb6-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-133">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-133">Monitor</span></span>

* <span data-ttu-id="efdb6-134">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="efdb6-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="efdb6-135">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="efdb6-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="efdb6-136">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="efdb6-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-137">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-137">Network</span></span>

* <span data-ttu-id="efdb6-138">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="efdb6-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-139">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-139">Profile</span></span>

* <span data-ttu-id="efdb6-140">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="efdb6-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="efdb6-141">SGBDR</span><span class="sxs-lookup"><span data-stu-id="efdb6-141">RDBMS</span></span>

* <span data-ttu-id="efdb6-142">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="efdb6-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-143">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-143">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="efdb6-145">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-145">Role</span></span>

* <span data-ttu-id="efdb6-146">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="efdb6-147">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="efdb6-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="efdb6-148">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="efdb6-149">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="efdb6-150">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="efdb6-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-151">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-151">Storage</span></span>

* <span data-ttu-id="efdb6-152">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="efdb6-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="efdb6-153">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="efdb6-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-154">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-154">VM</span></span>

* <span data-ttu-id="efdb6-155">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="efdb6-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="efdb6-156">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="efdb6-157">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="efdb6-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="efdb6-158">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="efdb6-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="efdb6-159">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-159">March 13, 2018</span></span>

<span data-ttu-id="efdb6-160">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="efdb6-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="efdb6-161">ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-161">ACR</span></span>

* <span data-ttu-id="efdb6-162">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="efdb6-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="efdb6-163">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="efdb6-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="efdb6-164">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="efdb6-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-165">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-165">ACS</span></span>

* <span data-ttu-id="efdb6-166">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="efdb6-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="efdb6-167">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="efdb6-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="efdb6-168">Advisor</span><span class="sxs-lookup"><span data-stu-id="efdb6-168">Advisor</span></span>

* <span data-ttu-id="efdb6-169">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="efdb6-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="efdb6-170">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="efdb6-171">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="efdb6-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="efdb6-172">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="efdb6-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="efdb6-173">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-174">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-174">Appservice</span></span>

* <span data-ttu-id="efdb6-175">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="efdb6-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="efdb6-176">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="efdb6-177">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="efdb6-177">Eventhubs</span></span>

* <span data-ttu-id="efdb6-178">Version initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="efdb6-179">Extension</span><span class="sxs-lookup"><span data-stu-id="efdb6-179">Extension</span></span>

* <span data-ttu-id="efdb6-180">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="efdb6-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-181">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-181">Interactive</span></span>

* <span data-ttu-id="efdb6-182">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="efdb6-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="efdb6-183">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="efdb6-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="efdb6-184">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="efdb6-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="efdb6-185">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="efdb6-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-186">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-186">Monitor</span></span>

* <span data-ttu-id="efdb6-187">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="efdb6-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="efdb6-188">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="efdb6-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="efdb6-189">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="efdb6-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="efdb6-190">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="efdb6-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-191">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-191">Network</span></span>

* <span data-ttu-id="efdb6-192">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="efdb6-193">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="efdb6-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="efdb6-194">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="efdb6-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="efdb6-195">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="efdb6-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-196">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-196">Profile</span></span>

* <span data-ttu-id="efdb6-197">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="efdb6-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="efdb6-198">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="efdb6-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="efdb6-199">SGBDR</span><span class="sxs-lookup"><span data-stu-id="efdb6-199">RDBMS</span></span>

* <span data-ttu-id="efdb6-200">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="efdb6-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="efdb6-201">Service Bus</span><span class="sxs-lookup"><span data-stu-id="efdb6-201">Service Bus</span></span>

* <span data-ttu-id="efdb6-202">Version initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-203">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-203">Storage</span></span>

* <span data-ttu-id="efdb6-204">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="efdb6-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="efdb6-205">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="efdb6-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-206">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-206">VM</span></span>

* <span data-ttu-id="efdb6-207">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="efdb6-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="efdb6-208">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="efdb6-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="efdb6-209">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="efdb6-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="efdb6-210">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="efdb6-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="efdb6-211">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-211">February 27, 2018</span></span>

<span data-ttu-id="efdb6-212">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="efdb6-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-213">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-213">Core</span></span>

* <span data-ttu-id="efdb6-214">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="efdb6-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="efdb6-215">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="efdb6-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="efdb6-216">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="efdb6-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-217">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-217">ACS</span></span>

* <span data-ttu-id="efdb6-218">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="efdb6-219">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="efdb6-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="efdb6-220">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="efdb6-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="efdb6-221">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="efdb6-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-222">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-222">Appservice</span></span>

* <span data-ttu-id="efdb6-223">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="efdb6-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="efdb6-224">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="efdb6-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="efdb6-225">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="efdb6-225">Cognitive Services</span></span>

* <span data-ttu-id="efdb6-226">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="efdb6-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="efdb6-227">Consommation</span><span class="sxs-lookup"><span data-stu-id="efdb6-227">Consumption</span></span>

* <span data-ttu-id="efdb6-228">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="efdb6-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="efdb6-229">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="efdb6-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-230">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-230">Container</span></span>

* <span data-ttu-id="efdb6-231">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="efdb6-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-232">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-232">Network</span></span>

* <span data-ttu-id="efdb6-233">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="efdb6-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-234">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-234">Resource</span></span>

* <span data-ttu-id="efdb6-235">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="efdb6-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-236">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-236">Role</span></span>

* <span data-ttu-id="efdb6-237">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="efdb6-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-238">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-238">SQL</span></span>

* <span data-ttu-id="efdb6-239">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="efdb6-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-240">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-240">Storage</span></span>

* <span data-ttu-id="efdb6-241">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-242">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-242">VM</span></span>

* <span data-ttu-id="efdb6-243">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="efdb6-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="efdb6-244">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-244">February 13, 2018</span></span>

<span data-ttu-id="efdb6-245">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="efdb6-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-246">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-246">Core</span></span>

* <span data-ttu-id="efdb6-247">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="efdb6-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-248">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-248">ACS</span></span>

* <span data-ttu-id="efdb6-249">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="efdb6-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="efdb6-250">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="efdb6-251">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="efdb6-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="efdb6-252">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="efdb6-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="efdb6-253">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="efdb6-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="efdb6-254">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="efdb6-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="efdb6-255">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="efdb6-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="efdb6-256">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="efdb6-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-257">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-257">Appservice</span></span>

* <span data-ttu-id="efdb6-258">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="efdb6-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="efdb6-259">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="efdb6-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="efdb6-260">CDN</span><span class="sxs-lookup"><span data-stu-id="efdb6-260">CDN</span></span>

* <span data-ttu-id="efdb6-261">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-262">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-262">Container</span></span>

* <span data-ttu-id="efdb6-263">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="efdb6-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="efdb6-264">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="efdb6-265">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="efdb6-265">CosmosDB</span></span>

* <span data-ttu-id="efdb6-266">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="efdb6-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="efdb6-267">Extension</span><span class="sxs-lookup"><span data-stu-id="efdb6-267">Extension</span></span>

* <span data-ttu-id="efdb6-268">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="efdb6-269">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="efdb6-270">Commentaires</span><span class="sxs-lookup"><span data-stu-id="efdb6-270">Feedback</span></span>

* <span data-ttu-id="efdb6-271">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="efdb6-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-272">Interactive</span></span>

* <span data-ttu-id="efdb6-273">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="efdb6-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="efdb6-274">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="efdb6-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="efdb6-275">IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-275">IoT</span></span>

* <span data-ttu-id="efdb6-276">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="efdb6-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="efdb6-277">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="efdb6-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="efdb6-278">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="efdb6-279">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="efdb6-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-280">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-280">Monitor</span></span>

* <span data-ttu-id="efdb6-281">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-282">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-282">Network</span></span>

* <span data-ttu-id="efdb6-283">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="efdb6-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="efdb6-284">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-284">Profile</span></span>

* <span data-ttu-id="efdb6-285">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="efdb6-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-286">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-286">Resource</span></span>

* <span data-ttu-id="efdb6-287">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-288">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-288">Role</span></span>

* <span data-ttu-id="efdb6-289">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-290">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-290">SQL</span></span>

* <span data-ttu-id="efdb6-291">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="efdb6-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="efdb6-292">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="efdb6-292">Added `sql db rename`</span></span>
* <span data-ttu-id="efdb6-293">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="efdb6-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-294">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-294">Storage</span></span>

* <span data-ttu-id="efdb6-295">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="efdb6-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-296">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-296">VM</span></span>

* <span data-ttu-id="efdb6-297">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="efdb6-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="efdb6-298">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="efdb6-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="efdb6-299">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="efdb6-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="efdb6-300">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-300">January 31, 2018</span></span>

<span data-ttu-id="efdb6-301">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="efdb6-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-302">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-302">Core</span></span>

* <span data-ttu-id="efdb6-303">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="efdb6-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="efdb6-304">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="efdb6-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="efdb6-305">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="efdb6-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="efdb6-306">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="efdb6-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="efdb6-307">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="efdb6-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-308">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-308">ACS</span></span>

* <span data-ttu-id="efdb6-309">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="efdb6-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="efdb6-310">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="efdb6-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-311">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-311">Appservice</span></span>

* <span data-ttu-id="efdb6-312">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="efdb6-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="efdb6-313">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="efdb6-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="efdb6-314">CDN</span><span class="sxs-lookup"><span data-stu-id="efdb6-314">CDN</span></span>

* <span data-ttu-id="efdb6-315">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="efdb6-316">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="efdb6-316">CosmosDB</span></span>

* <span data-ttu-id="efdb6-317">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="efdb6-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-318">Interactive</span></span>

* <span data-ttu-id="efdb6-319">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="efdb6-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-320">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-320">Network</span></span>

* <span data-ttu-id="efdb6-321">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="efdb6-322">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="efdb6-323">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="efdb6-324">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="efdb6-325">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="efdb6-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="efdb6-326">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="efdb6-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="efdb6-327">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="efdb6-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="efdb6-328">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="efdb6-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="efdb6-329">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="efdb6-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="efdb6-330">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="efdb6-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-331">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-331">Profile</span></span>

* <span data-ttu-id="efdb6-332">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="efdb6-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-333">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-333">Resource</span></span>

* <span data-ttu-id="efdb6-334">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="efdb6-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-335">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-335">Storage</span></span>

* <span data-ttu-id="efdb6-336">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="efdb6-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="efdb6-337">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="efdb6-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="efdb6-338">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="efdb6-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="efdb6-339">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="efdb6-340">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="efdb6-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-341">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-341">VM</span></span>

* <span data-ttu-id="efdb6-342">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="efdb6-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="efdb6-343">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="efdb6-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="efdb6-344">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="efdb6-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="efdb6-345">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="efdb6-346">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="efdb6-346">January 17, 2018</span></span>

<span data-ttu-id="efdb6-347">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="efdb6-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="efdb6-348">ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-348">ACR</span></span>

* <span data-ttu-id="efdb6-349">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="efdb6-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="efdb6-350">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="efdb6-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-351">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-351">ACS</span></span>

* <span data-ttu-id="efdb6-352">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="efdb6-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="efdb6-353">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="efdb6-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-354">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-354">Appservice</span></span>

* <span data-ttu-id="efdb6-355">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="efdb6-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="efdb6-356">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="efdb6-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="efdb6-357">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="efdb6-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="efdb6-358">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="efdb6-358">Backup</span></span>

* <span data-ttu-id="efdb6-359">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="efdb6-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="efdb6-360">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="efdb6-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="efdb6-361">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="efdb6-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="efdb6-362">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="efdb6-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="efdb6-363">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="efdb6-364">Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-364">Batch</span></span>

* <span data-ttu-id="efdb6-365">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="efdb6-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="efdb6-366">Cloud</span><span class="sxs-lookup"><span data-stu-id="efdb6-366">Cloud</span></span>

* <span data-ttu-id="efdb6-367">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="efdb6-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="efdb6-368">Consommation</span><span class="sxs-lookup"><span data-stu-id="efdb6-368">Consumption</span></span>

* <span data-ttu-id="efdb6-369">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="efdb6-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="efdb6-370">Event Grid</span><span class="sxs-lookup"><span data-stu-id="efdb6-370">Event Grid</span></span>

* <span data-ttu-id="efdb6-371">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="efdb6-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="efdb6-372">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="efdb6-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="efdb6-373">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="efdb6-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="efdb6-374">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="efdb6-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="efdb6-375">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="efdb6-376">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="efdb6-377">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="efdb6-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="efdb6-378">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="efdb6-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-379">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-379">Interactive</span></span>

* <span data-ttu-id="efdb6-380">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="efdb6-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="efdb6-381">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="efdb6-381">Fixed errors on startup</span></span>
* <span data-ttu-id="efdb6-382">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="efdb6-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="efdb6-383">IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-383">IoT</span></span>

* <span data-ttu-id="efdb6-384">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="efdb6-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="efdb6-385">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="efdb6-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="efdb6-386">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-387">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-387">Monitor</span></span>

* <span data-ttu-id="efdb6-388">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="efdb6-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="efdb6-389">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="efdb6-390">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="efdb6-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-391">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-391">Network</span></span>

* <span data-ttu-id="efdb6-392">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="efdb6-393">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-394">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-394">Profile</span></span>

* <span data-ttu-id="efdb6-395">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="efdb6-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-396">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-396">Role</span></span>

* <span data-ttu-id="efdb6-397">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="efdb6-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="efdb6-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="efdb6-398">Service Fabric</span></span>

* <span data-ttu-id="efdb6-399">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="efdb6-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="efdb6-400">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="efdb6-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-401">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-401">VM</span></span>

* <span data-ttu-id="efdb6-402">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="efdb6-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="efdb6-403">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="efdb6-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="efdb6-404">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="efdb6-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="efdb6-405">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="efdb6-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="efdb6-406">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="efdb6-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="efdb6-407">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="efdb6-408">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="efdb6-409">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="efdb6-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="efdb6-410">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-410">December 19, 2017</span></span>

<span data-ttu-id="efdb6-411">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="efdb6-411">Version 2.0.23</span></span>

* <span data-ttu-id="efdb6-412">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="efdb6-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-413">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-413">Container</span></span>

* <span data-ttu-id="efdb6-414">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-415">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-415">Network</span></span>

* <span data-ttu-id="efdb6-416">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="efdb6-417">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-418">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-418">Storage</span></span>

* <span data-ttu-id="efdb6-419">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="efdb6-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-420">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-420">VM</span></span>

* <span data-ttu-id="efdb6-421">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="efdb6-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="efdb6-422">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-422">December 5, 2017</span></span>

<span data-ttu-id="efdb6-423">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="efdb6-423">Version 2.0.22</span></span>

* <span data-ttu-id="efdb6-424">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="efdb6-424">Removed `az component` commands.</span></span> <span data-ttu-id="efdb6-425">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="efdb6-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-426">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-426">Core</span></span>
* <span data-ttu-id="efdb6-427">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="efdb6-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="efdb6-428">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="efdb6-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-429">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-429">ACS</span></span>

* <span data-ttu-id="efdb6-430">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="efdb6-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="efdb6-431">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="efdb6-432">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="efdb6-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="efdb6-433">Advisor</span><span class="sxs-lookup"><span data-stu-id="efdb6-433">Advisor</span></span>

* <span data-ttu-id="efdb6-434">Version initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-435">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-435">Appservice</span></span>

* <span data-ttu-id="efdb6-436">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="efdb6-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="efdb6-437">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="efdb6-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="efdb6-438">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="efdb6-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="efdb6-439">Consommation</span><span class="sxs-lookup"><span data-stu-id="efdb6-439">Consumption</span></span>

* <span data-ttu-id="efdb6-440">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="efdb6-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-441">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-441">Container</span></span>

* <span data-ttu-id="efdb6-442">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-443">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-443">Monitor</span></span>

* <span data-ttu-id="efdb6-444">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="efdb6-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-445">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-445">Resource</span></span>

* <span data-ttu-id="efdb6-446">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-447">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-447">Role</span></span>

* <span data-ttu-id="efdb6-448">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="efdb6-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="efdb6-449">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="efdb6-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="efdb6-450">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="efdb6-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-451">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-451">SQL</span></span>

* <span data-ttu-id="efdb6-452">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="efdb6-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="efdb6-453">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-454">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-454">VM</span></span>

* <span data-ttu-id="efdb6-455">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="efdb6-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="efdb6-456">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-456">November 14, 2017</span></span>

<span data-ttu-id="efdb6-457">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="efdb6-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="efdb6-458">ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-458">ACR</span></span>

* <span data-ttu-id="efdb6-459">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="efdb6-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="efdb6-460">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-460">ACS</span></span>

* <span data-ttu-id="efdb6-461">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="efdb6-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="efdb6-462">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="efdb6-463">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="efdb6-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="efdb6-464">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="efdb6-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="efdb6-465">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="efdb6-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-466">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-466">Appservice</span></span>

* <span data-ttu-id="efdb6-467">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="efdb6-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="efdb6-468">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="efdb6-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="efdb6-469">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="efdb6-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="efdb6-470">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="efdb6-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="efdb6-471">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="efdb6-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="efdb6-472">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="efdb6-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="efdb6-473">Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-473">Batch</span></span>

* <span data-ttu-id="efdb6-474">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="efdb6-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="efdb6-475">Batchai</span><span class="sxs-lookup"><span data-stu-id="efdb6-475">Batchai</span></span>

* <span data-ttu-id="efdb6-476">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="efdb6-477">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="efdb6-478">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="efdb6-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="efdb6-479">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="efdb6-480">Cloud</span><span class="sxs-lookup"><span data-stu-id="efdb6-480">Cloud</span></span>

* <span data-ttu-id="efdb6-481">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="efdb6-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-482">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-482">Container</span></span>

* <span data-ttu-id="efdb6-483">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="efdb6-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="efdb6-484">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="efdb6-484">Added container group restart policy</span></span>
* <span data-ttu-id="efdb6-485">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="efdb6-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="efdb6-486">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="efdb6-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="efdb6-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="efdb6-487">Data Lake Analytics</span></span>

* <span data-ttu-id="efdb6-488">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="efdb6-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="efdb6-489">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-489">Data Lake Store</span></span>

* <span data-ttu-id="efdb6-490">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="efdb6-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="efdb6-491">Extension</span><span class="sxs-lookup"><span data-stu-id="efdb6-491">Extension</span></span>

* <span data-ttu-id="efdb6-492">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="efdb6-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="efdb6-493">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="efdb6-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="efdb6-494">IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-494">IoT</span></span>

* <span data-ttu-id="efdb6-495">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="efdb6-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-496">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-496">Monitor</span></span>

* <span data-ttu-id="efdb6-497">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="efdb6-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-498">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-498">Network</span></span>

* <span data-ttu-id="efdb6-499">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="efdb6-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="efdb6-500">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="efdb6-501">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="efdb6-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="efdb6-502">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="efdb6-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="efdb6-503">Réservations</span><span class="sxs-lookup"><span data-stu-id="efdb6-503">Reservations</span></span>

* <span data-ttu-id="efdb6-504">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-505">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-505">Resource</span></span>

* <span data-ttu-id="efdb6-506">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="efdb6-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-507">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-507">SQL</span></span>

* <span data-ttu-id="efdb6-508">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-509">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-509">Storage</span></span>

* <span data-ttu-id="efdb6-510">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="efdb6-511">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="efdb6-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="efdb6-512">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="efdb6-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="efdb6-513">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="efdb6-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="efdb6-514">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="efdb6-515">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="efdb6-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="efdb6-516">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-517">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-517">VM</span></span>

* <span data-ttu-id="efdb6-518">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="efdb6-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="efdb6-519">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="efdb6-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="efdb6-520">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="efdb6-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="efdb6-521">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="efdb6-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="efdb6-522">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="efdb6-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="efdb6-523">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-523">October 24, 2017</span></span>

<span data-ttu-id="efdb6-524">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="efdb6-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-525">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-525">Core</span></span>

* <span data-ttu-id="efdb6-526">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="efdb6-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="efdb6-527">ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-527">ACR</span></span>

* <span data-ttu-id="efdb6-528">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="efdb6-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="efdb6-529">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="efdb6-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="efdb6-530">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="efdb6-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-531">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-531">ACS</span></span>

* <span data-ttu-id="efdb6-532">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="efdb6-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="efdb6-533">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="efdb6-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-534">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-534">Appservice</span></span>

* <span data-ttu-id="efdb6-535">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="efdb6-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="efdb6-536">Composant</span><span class="sxs-lookup"><span data-stu-id="efdb6-536">Component</span></span>

* <span data-ttu-id="efdb6-537">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="efdb6-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-538">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-538">Monitor</span></span>

* <span data-ttu-id="efdb6-539">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="efdb6-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-540">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-540">Resource</span></span>

* <span data-ttu-id="efdb6-541">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="efdb6-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="efdb6-542">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="efdb6-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-543">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-543">VM</span></span>

* <span data-ttu-id="efdb6-544">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="efdb6-545">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-545">October 9, 2017</span></span>

<span data-ttu-id="efdb6-546">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="efdb6-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-547">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-547">Core</span></span>

* <span data-ttu-id="efdb6-548">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="efdb6-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-549">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-549">Appservice</span></span>

* <span data-ttu-id="efdb6-550">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="efdb6-551">Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-551">Batch</span></span>

* <span data-ttu-id="efdb6-552">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="efdb6-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="efdb6-553">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="efdb6-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="efdb6-554">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="efdb6-555">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="efdb6-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="efdb6-556">Batchai</span><span class="sxs-lookup"><span data-stu-id="efdb6-556">Batchai</span></span>

* <span data-ttu-id="efdb6-557">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="efdb6-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="efdb6-558">KeyVault</span><span class="sxs-lookup"><span data-stu-id="efdb6-558">Keyvault</span></span>

* <span data-ttu-id="efdb6-559">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="efdb6-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="efdb6-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="efdb6-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="efdb6-561">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-561">Network</span></span>

* <span data-ttu-id="efdb6-562">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="efdb6-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="efdb6-563">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="efdb6-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-564">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-564">Resource</span></span>

* <span data-ttu-id="efdb6-565">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="efdb6-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="efdb6-566">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="efdb6-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="efdb6-567">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="efdb6-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="efdb6-568">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="efdb6-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-569">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-569">Sql</span></span>

* <span data-ttu-id="efdb6-570">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="efdb6-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="efdb6-571">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="efdb6-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="efdb6-572">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="efdb6-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-573">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-573">Storage</span></span>

* <span data-ttu-id="efdb6-574">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="efdb6-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-575">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-575">Vm</span></span>

* <span data-ttu-id="efdb6-576">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="efdb6-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="efdb6-577">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="efdb6-578">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="efdb6-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="efdb6-579">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="efdb6-580">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="efdb6-581">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-581">September 22, 2017</span></span>

<span data-ttu-id="efdb6-582">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="efdb6-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-583">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-583">Resource</span></span>

* <span data-ttu-id="efdb6-584">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="efdb6-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="efdb6-585">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="efdb6-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="efdb6-586">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="efdb6-587">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="efdb6-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-588">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-588">Network</span></span>

* <span data-ttu-id="efdb6-589">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="efdb6-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="efdb6-590">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="efdb6-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="efdb6-591">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="efdb6-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="efdb6-592">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="efdb6-593">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="efdb6-594">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="efdb6-595">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-596">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-596">Storage</span></span>

* <span data-ttu-id="efdb6-597">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="efdb6-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="efdb6-598">Événement</span><span class="sxs-lookup"><span data-stu-id="efdb6-598">Eventgrid</span></span>

* <span data-ttu-id="efdb6-599">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="efdb6-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-600">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-600">SQL</span></span>

* <span data-ttu-id="efdb6-601">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="efdb6-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="efdb6-602">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="efdb6-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="efdb6-603">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="efdb6-604">KeyVault</span><span class="sxs-lookup"><span data-stu-id="efdb6-604">Keyvault</span></span>

* <span data-ttu-id="efdb6-605">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="efdb6-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-606">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-606">VM</span></span>

* <span data-ttu-id="efdb6-607">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="efdb6-608">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="efdb6-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="efdb6-609">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="efdb6-610">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="efdb6-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="efdb6-611">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="efdb6-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="efdb6-612">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="efdb6-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-613">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-613">ACS</span></span>

* <span data-ttu-id="efdb6-614">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="efdb6-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-615">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-615">Appservice</span></span>

* <span data-ttu-id="efdb6-616">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="efdb6-617">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="efdb6-617">Backup</span></span>

* <span data-ttu-id="efdb6-618">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="efdb6-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="efdb6-619">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-619">September 11, 2017</span></span>

<span data-ttu-id="efdb6-620">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="efdb6-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="efdb6-621">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-621">Core</span></span>

* <span data-ttu-id="efdb6-622">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="efdb6-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="efdb6-623">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="efdb6-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-624">Acs</span><span class="sxs-lookup"><span data-stu-id="efdb6-624">Acs</span></span>

* <span data-ttu-id="efdb6-625">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="efdb6-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="efdb6-626">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="efdb6-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-627">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-627">Appservice</span></span>

* <span data-ttu-id="efdb6-628">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="efdb6-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="efdb6-629">CDN</span><span class="sxs-lookup"><span data-stu-id="efdb6-629">CDN</span></span>

* <span data-ttu-id="efdb6-630">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="efdb6-631">Extension</span><span class="sxs-lookup"><span data-stu-id="efdb6-631">Extension</span></span>

* <span data-ttu-id="efdb6-632">Version initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="efdb6-633">KeyVault</span><span class="sxs-lookup"><span data-stu-id="efdb6-633">Keyvault</span></span>

* <span data-ttu-id="efdb6-634">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="efdb6-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-635">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-635">Network</span></span>

* <span data-ttu-id="efdb6-636">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="efdb6-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="efdb6-637">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="efdb6-638">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="efdb6-639">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="efdb6-640">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-641">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-641">Resource</span></span>

* <span data-ttu-id="efdb6-642">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="efdb6-643">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="efdb6-644">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="efdb6-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="efdb6-645">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="efdb6-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-646">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-646">SQL</span></span>

* <span data-ttu-id="efdb6-647">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="efdb6-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-648">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-648">VM</span></span>

* <span data-ttu-id="efdb6-649">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="efdb6-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="efdb6-650">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="efdb6-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="efdb6-651">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="efdb6-652">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="efdb6-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="efdb6-653">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="efdb6-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="efdb6-654">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-654">August 31, 2017</span></span>

<span data-ttu-id="efdb6-655">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="efdb6-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="efdb6-656">KeyVault</span><span class="sxs-lookup"><span data-stu-id="efdb6-656">Keyvault</span></span>

* <span data-ttu-id="efdb6-657">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="efdb6-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="efdb6-658">Sf</span><span class="sxs-lookup"><span data-stu-id="efdb6-658">Sf</span></span>

* <span data-ttu-id="efdb6-659">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="efdb6-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-660">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-660">Storage</span></span>

* <span data-ttu-id="efdb6-661">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="efdb6-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="efdb6-662">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="efdb6-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="efdb6-663">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-663">August 28, 2017</span></span>

<span data-ttu-id="efdb6-664">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="efdb6-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="efdb6-665">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="efdb6-665">CLI</span></span>

* <span data-ttu-id="efdb6-666">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="efdb6-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-667">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-667">ACS</span></span>

* <span data-ttu-id="efdb6-668">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="efdb6-668">Corrected preview regions</span></span>
* <span data-ttu-id="efdb6-669">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="efdb6-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="efdb6-670">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-671">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-671">Appservice</span></span>

* <span data-ttu-id="efdb6-672">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="efdb6-673">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="efdb6-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="efdb6-674">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="efdb6-675">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="efdb6-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="efdb6-676">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="efdb6-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="efdb6-677">IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-677">IoT</span></span>

* <span data-ttu-id="efdb6-678">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="efdb6-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-679">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-679">Network</span></span>

* <span data-ttu-id="efdb6-680">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="efdb6-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="efdb6-681">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="efdb6-682">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="efdb6-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="efdb6-683">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="efdb6-684">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-685">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-685">Profile</span></span>

* <span data-ttu-id="efdb6-686">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="efdb6-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="efdb6-687">Service Fabric</span></span>

* <span data-ttu-id="efdb6-688">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="efdb6-688">Preview release</span></span>
* <span data-ttu-id="efdb6-689">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="efdb6-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="efdb6-690">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="efdb6-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="efdb6-691">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="efdb6-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-692">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-692">Storage</span></span>

* <span data-ttu-id="efdb6-693">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="efdb6-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="efdb6-694">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="efdb6-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="efdb6-695">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="efdb6-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="efdb6-696">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="efdb6-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="efdb6-697">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="efdb6-698">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="efdb6-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-699">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-699">VM</span></span>

* <span data-ttu-id="efdb6-700">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="efdb6-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="efdb6-701">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="efdb6-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="efdb6-702">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="efdb6-703">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="efdb6-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="efdb6-704">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="efdb6-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="efdb6-705">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="efdb6-706">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-706">August 15, 2017</span></span>

<span data-ttu-id="efdb6-707">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="efdb6-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-708">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-708">ACS</span></span>

* <span data-ttu-id="efdb6-709">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="efdb6-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-710">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-710">Appservice</span></span>

* <span data-ttu-id="efdb6-711">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="efdb6-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="efdb6-712">Event Grid</span><span class="sxs-lookup"><span data-stu-id="efdb6-712">Event Grid</span></span>

* <span data-ttu-id="efdb6-713">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="efdb6-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="efdb6-714">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-714">August 11, 2017</span></span>

<span data-ttu-id="efdb6-715">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="efdb6-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-716">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-716">ACS</span></span>

* <span data-ttu-id="efdb6-717">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="efdb6-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="efdb6-718">Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-718">Batch</span></span>

* <span data-ttu-id="efdb6-719">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="efdb6-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="efdb6-720">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="efdb6-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="efdb6-721">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="efdb6-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="efdb6-722">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="efdb6-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="efdb6-723">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="efdb6-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="efdb6-724">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="efdb6-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="efdb6-725">Composant</span><span class="sxs-lookup"><span data-stu-id="efdb6-725">Component</span></span>

* <span data-ttu-id="efdb6-726">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="efdb6-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="efdb6-727">Conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-727">Container</span></span>

* <span data-ttu-id="efdb6-728">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="efdb6-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="efdb6-729">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-729">Data Lake Store</span></span>

* <span data-ttu-id="efdb6-730">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="efdb6-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="efdb6-731">Event Grid</span><span class="sxs-lookup"><span data-stu-id="efdb6-731">Event Grid</span></span>

* <span data-ttu-id="efdb6-732">Version initiale</span><span class="sxs-lookup"><span data-stu-id="efdb6-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-733">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-733">Network</span></span>

* <span data-ttu-id="efdb6-734">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="efdb6-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="efdb6-735">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="efdb6-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="efdb6-736">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="efdb6-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="efdb6-737">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="efdb6-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-738">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-738">Profile</span></span>

* <span data-ttu-id="efdb6-739">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="efdb6-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-740">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-740">Storage</span></span>

* <span data-ttu-id="efdb6-741">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="efdb6-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-742">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-742">VM</span></span>

* <span data-ttu-id="efdb6-743">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="efdb6-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="efdb6-744">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="efdb6-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="efdb6-745">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="efdb6-746">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="efdb6-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="efdb6-747">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="efdb6-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="efdb6-748">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-748">July 28, 2017</span></span>

<span data-ttu-id="efdb6-749">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="efdb6-749">Version 2.0.12</span></span>

* <span data-ttu-id="efdb6-750">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="efdb6-750">Added container commands</span></span>
* <span data-ttu-id="efdb6-751">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="efdb6-751">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="efdb6-752">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-752">Core</span></span>

* <span data-ttu-id="efdb6-753">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="efdb6-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="efdb6-754">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="efdb6-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="efdb6-755">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="efdb6-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="efdb6-756">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="efdb6-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="efdb6-757">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="efdb6-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="efdb6-758">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="efdb6-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="efdb6-759">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="efdb6-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="efdb6-760">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="efdb6-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="efdb6-761">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="efdb6-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="efdb6-762">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="efdb6-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="efdb6-763">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="efdb6-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="efdb6-764">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="efdb6-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="efdb6-765">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="efdb6-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="efdb6-766">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="efdb6-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="efdb6-767">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="efdb6-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="efdb6-768">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="efdb6-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="efdb6-769">ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-769">ACR</span></span>

* <span data-ttu-id="efdb6-770">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="efdb6-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="efdb6-771">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="efdb6-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="efdb6-772">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="efdb6-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="efdb6-773">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="efdb6-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="efdb6-774">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="efdb6-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="efdb6-775">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="efdb6-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-776">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-776">ACS</span></span>

* <span data-ttu-id="efdb6-777">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="efdb6-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-778">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-778">Appservice</span></span>

* <span data-ttu-id="efdb6-779">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="efdb6-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="efdb6-780">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="efdb6-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="efdb6-781">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="efdb6-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="efdb6-782">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="efdb6-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="efdb6-783">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="efdb6-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="efdb6-784">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="efdb6-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="efdb6-785">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="efdb6-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="efdb6-786">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="efdb6-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="efdb6-787">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="efdb6-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="efdb6-788">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="efdb6-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="efdb6-789">Batch</span><span class="sxs-lookup"><span data-stu-id="efdb6-789">Batch</span></span>

* <span data-ttu-id="efdb6-790">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="efdb6-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="efdb6-791">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="efdb6-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="efdb6-792">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="efdb6-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="efdb6-793">CDN</span><span class="sxs-lookup"><span data-stu-id="efdb6-793">CDN</span></span>

* <span data-ttu-id="efdb6-794">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="efdb6-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="efdb6-795">Cloud</span><span class="sxs-lookup"><span data-stu-id="efdb6-795">Cloud</span></span>

* <span data-ttu-id="efdb6-796">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="efdb6-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="efdb6-797">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="efdb6-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="efdb6-798">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="efdb6-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="efdb6-799">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="efdb6-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="efdb6-800">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="efdb6-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="efdb6-801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="efdb6-801">CosmosDB</span></span>

* <span data-ttu-id="efdb6-802">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="efdb6-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="efdb6-803">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="efdb6-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="efdb6-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="efdb6-804">Data Lake Analytics</span></span>

* <span data-ttu-id="efdb6-805">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="efdb6-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="efdb6-806">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="efdb6-807">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="efdb6-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="efdb6-808">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-808">Data Lake Store</span></span>

* <span data-ttu-id="efdb6-809">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="efdb6-810">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="efdb6-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="efdb6-811">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="efdb6-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="efdb6-812">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="efdb6-813">Interactive</span><span class="sxs-lookup"><span data-stu-id="efdb6-813">Interactive</span></span>

* <span data-ttu-id="efdb6-814">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="efdb6-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="efdb6-815">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="efdb6-815">Increased test coverage</span></span>
* <span data-ttu-id="efdb6-816">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="efdb6-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="efdb6-817">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="efdb6-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="efdb6-818">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="efdb6-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="efdb6-819">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="efdb6-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="efdb6-820">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="efdb6-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="efdb6-821">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="efdb6-821">Added `--progress` flag</span></span>
* <span data-ttu-id="efdb6-822">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="efdb6-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="efdb6-823">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="efdb6-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="efdb6-824">IoT</span><span class="sxs-lookup"><span data-stu-id="efdb6-824">IoT</span></span>

* <span data-ttu-id="efdb6-825">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="efdb6-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="efdb6-826">(#3934)</span><span class="sxs-lookup"><span data-stu-id="efdb6-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="efdb6-827">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="efdb6-827">Key vault</span></span>

* <span data-ttu-id="efdb6-828">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="efdb6-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="efdb6-829">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="efdb6-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="efdb6-830">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="efdb6-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="efdb6-831">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="efdb6-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="efdb6-832">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="efdb6-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="efdb6-833">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="efdb6-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="efdb6-834">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="efdb6-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="efdb6-835">(#3307)</span><span class="sxs-lookup"><span data-stu-id="efdb6-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="efdb6-836">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-836">Lab</span></span>

* <span data-ttu-id="efdb6-837">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="efdb6-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="efdb6-838">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-839">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-839">Monitor</span></span>

* <span data-ttu-id="efdb6-840">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="efdb6-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="efdb6-841">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="efdb6-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="efdb6-842">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="efdb6-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="efdb6-843">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="efdb6-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="efdb6-844">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="efdb6-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="efdb6-845">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="efdb6-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="efdb6-846">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="efdb6-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="efdb6-847">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="efdb6-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="efdb6-848">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="efdb6-848">`location` no longer required</span></span>
  * <span data-ttu-id="efdb6-849">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="efdb6-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="efdb6-850">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="efdb6-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="efdb6-851">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="efdb6-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="efdb6-852">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="efdb6-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="efdb6-853">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="efdb6-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="efdb6-854">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="efdb6-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="efdb6-855">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-856">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-856">Network</span></span>

* <span data-ttu-id="efdb6-857">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="efdb6-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="efdb6-858">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="efdb6-859">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="efdb6-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="efdb6-860">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="efdb6-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="efdb6-861">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="efdb6-862">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="efdb6-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="efdb6-863">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="efdb6-864">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="efdb6-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="efdb6-865">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="efdb6-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="efdb6-866">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="efdb6-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="efdb6-867">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="efdb6-868">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="efdb6-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="efdb6-869">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="efdb6-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="efdb6-870">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="efdb6-871">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="efdb6-872">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="efdb6-873">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="efdb6-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="efdb6-874">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="efdb6-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="efdb6-875">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="efdb6-876">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="efdb6-877">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="efdb6-878">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="efdb6-879">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="efdb6-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="efdb6-880">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="efdb6-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="efdb6-881">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="efdb6-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="efdb6-882">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="efdb6-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="efdb6-883">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="efdb6-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-884">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-884">Profile</span></span>

* <span data-ttu-id="efdb6-885">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="efdb6-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="efdb6-886">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="efdb6-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="efdb6-887">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="efdb6-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="efdb6-888">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="efdb6-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="efdb6-889">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="efdb6-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="efdb6-890">SGBDR</span><span class="sxs-lookup"><span data-stu-id="efdb6-890">RDBMS</span></span>

* <span data-ttu-id="efdb6-891">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="efdb6-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="efdb6-892">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="efdb6-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="efdb6-893">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="efdb6-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="efdb6-894">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="efdb6-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-895">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-895">Resource</span></span>

* <span data-ttu-id="efdb6-896">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="efdb6-897">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="efdb6-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="efdb6-898">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="efdb6-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="efdb6-899">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="efdb6-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="efdb6-900">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="efdb6-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="efdb6-901">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="efdb6-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="efdb6-902">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="efdb6-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="efdb6-903">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="efdb6-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-904">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-904">Role</span></span>

* <span data-ttu-id="efdb6-905">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="efdb6-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="efdb6-906">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="efdb6-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="efdb6-907">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="efdb6-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="efdb6-908">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="efdb6-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="efdb6-909">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="efdb6-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="efdb6-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="efdb6-910">Service Fabric</span></span>
* <span data-ttu-id="efdb6-911">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="efdb6-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="efdb6-912">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="efdb6-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="efdb6-913">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="efdb6-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-914">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-914">SQL</span></span>

* <span data-ttu-id="efdb6-915">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="efdb6-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="efdb6-916">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="efdb6-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="efdb6-917">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="efdb6-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-918">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-918">Storage</span></span>

* <span data-ttu-id="efdb6-919">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="efdb6-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="efdb6-920">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="efdb6-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="efdb6-921">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="efdb6-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="efdb6-922">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="efdb6-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="efdb6-923">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="efdb6-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="efdb6-924">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="efdb6-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-925">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-925">VM</span></span>

* <span data-ttu-id="efdb6-926">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-926">Support configuring nsg</span></span>
* <span data-ttu-id="efdb6-927">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="efdb6-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="efdb6-928">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="efdb6-928">Support managed service identities</span></span>
* <span data-ttu-id="efdb6-929">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="efdb6-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="efdb6-930">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="efdb6-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="efdb6-931">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-931">May 10, 2017</span></span>

<span data-ttu-id="efdb6-932">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="efdb6-932">Version 2.0.6</span></span>

* <span data-ttu-id="efdb6-933">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="efdb6-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="efdb6-934">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="efdb6-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="efdb6-935">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="efdb6-936">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="efdb6-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="efdb6-937">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="efdb6-937">Include Service Fabric module</span></span>
* <span data-ttu-id="efdb6-938">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="efdb6-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="efdb6-939">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="efdb6-939">Add support for CDN commands</span></span>
* <span data-ttu-id="efdb6-940">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="efdb6-940">Remove Container module</span></span>
* <span data-ttu-id="efdb6-941">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="efdb6-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="efdb6-942">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="efdb6-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="efdb6-943">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-943">Core</span></span>

* <span data-ttu-id="efdb6-944">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="efdb6-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="efdb6-945">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="efdb6-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="efdb6-946">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="efdb6-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="efdb6-947">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="efdb6-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="efdb6-948">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="efdb6-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="efdb6-949">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="efdb6-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="efdb6-950">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="efdb6-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="efdb6-951">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="efdb6-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="efdb6-952">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="efdb6-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="efdb6-953">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="efdb6-953">core: Improved performance</span></span>
* <span data-ttu-id="efdb6-954">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="efdb6-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="efdb6-955">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="efdb6-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-956">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-956">ACS</span></span>

* <span data-ttu-id="efdb6-957">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="efdb6-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="efdb6-958">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="efdb6-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="efdb6-959">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="efdb6-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="efdb6-960">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="efdb6-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-961">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-961">AppService</span></span>

* <span data-ttu-id="efdb6-962">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="efdb6-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="efdb6-963">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="efdb6-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="efdb6-964">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="efdb6-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="efdb6-965">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="efdb6-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="efdb6-966">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="efdb6-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="efdb6-967">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="efdb6-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="efdb6-968">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="efdb6-968">support slot swap with preview</span></span>
* <span data-ttu-id="efdb6-969">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="efdb6-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="efdb6-970">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="efdb6-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="efdb6-971">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="efdb6-971">CosmosDB</span></span>

* <span data-ttu-id="efdb6-972">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="efdb6-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="efdb6-973">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="efdb6-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="efdb6-974">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="efdb6-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="efdb6-975">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="efdb6-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="efdb6-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="efdb6-976">Data Lake Analytics</span></span>

* <span data-ttu-id="efdb6-977">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="efdb6-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="efdb6-978">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="efdb6-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="efdb6-979">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="efdb6-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="efdb6-980">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="efdb6-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="efdb6-981">Table</span><span class="sxs-lookup"><span data-stu-id="efdb6-981">Table</span></span>
  * <span data-ttu-id="efdb6-982">Fonction table</span><span class="sxs-lookup"><span data-stu-id="efdb6-982">Table valued function</span></span>
  * <span data-ttu-id="efdb6-983">Affichage</span><span class="sxs-lookup"><span data-stu-id="efdb6-983">View</span></span>
  * <span data-ttu-id="efdb6-984">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="efdb6-984">Table Statistics.</span></span> <span data-ttu-id="efdb6-985">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="efdb6-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="efdb6-986">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-986">Data Lake Store</span></span>

* <span data-ttu-id="efdb6-987">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="efdb6-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="efdb6-988">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="efdb6-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="efdb6-989">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="efdb6-989">missed help for access show.</span></span> <span data-ttu-id="efdb6-990">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="efdb6-990">adding it.</span></span> <span data-ttu-id="efdb6-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="efdb6-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="efdb6-992">Rechercher</span><span class="sxs-lookup"><span data-stu-id="efdb6-992">Find</span></span>

* <span data-ttu-id="efdb6-993">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="efdb6-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="efdb6-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="efdb6-994">KeyVault</span></span>

* <span data-ttu-id="efdb6-995">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="efdb6-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="efdb6-996">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="efdb6-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="efdb6-997">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="efdb6-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="efdb6-998">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="efdb6-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="efdb6-999">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="efdb6-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="efdb6-1000">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1000">Lab</span></span>

* <span data-ttu-id="efdb6-1001">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="efdb6-1002">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="efdb6-1003">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="efdb6-1004">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="efdb6-1005">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="efdb6-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="efdb6-1006">Surveiller</span><span class="sxs-lookup"><span data-stu-id="efdb6-1006">Monitor</span></span>

* <span data-ttu-id="efdb6-1007">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="efdb6-1008">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="efdb6-1009">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-1009">Network</span></span>

* <span data-ttu-id="efdb6-1010">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="efdb6-1011">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="efdb6-1012">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="efdb6-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="efdb6-1013">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="efdb6-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="efdb6-1014">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="efdb6-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="efdb6-1015">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="efdb6-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="efdb6-1016">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="efdb6-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="efdb6-1017">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="efdb6-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="efdb6-1018">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="efdb6-1019">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="efdb6-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="efdb6-1020">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="efdb6-1021">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="efdb6-1022">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="efdb6-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="efdb6-1023">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="efdb6-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="efdb6-1024">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="efdb6-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="efdb6-1025">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="efdb6-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="efdb6-1026">Profil</span><span class="sxs-lookup"><span data-stu-id="efdb6-1026">Profile</span></span>

* <span data-ttu-id="efdb6-1027">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="efdb6-1028">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="efdb6-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="efdb6-1029">Redis</span></span>

* <span data-ttu-id="efdb6-1030">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="efdb6-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="efdb6-1031">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="efdb6-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="efdb6-1032">Ressource</span><span class="sxs-lookup"><span data-stu-id="efdb6-1032">Resource</span></span>

* <span data-ttu-id="efdb6-1033">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="efdb6-1034">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="efdb6-1035">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="efdb6-1036">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="efdb6-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="efdb6-1038">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1038">Add docs for az lock update.</span></span> <span data-ttu-id="efdb6-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="efdb6-1040">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="efdb6-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="efdb6-1042">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="efdb6-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="efdb6-1044">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="efdb6-1045">Rôle</span><span class="sxs-lookup"><span data-stu-id="efdb6-1045">Role</span></span>

* <span data-ttu-id="efdb6-1046">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="efdb6-1047">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="efdb6-1048">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="efdb6-1049">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="efdb6-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="efdb6-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="efdb6-1050">SQL</span></span>

* <span data-ttu-id="efdb6-1051">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="efdb6-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="efdb6-1052">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="efdb6-1053">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-1053">Storage</span></span>

* <span data-ttu-id="efdb6-1054">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="efdb6-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="efdb6-1055">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="efdb6-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="efdb6-1056">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="efdb6-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="efdb6-1057">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="efdb6-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-1058">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-1058">VM</span></span>

* <span data-ttu-id="efdb6-1059">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="efdb6-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="efdb6-1060">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="efdb6-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="efdb6-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="efdb6-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="efdb6-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="efdb6-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="efdb6-1063">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="efdb6-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="efdb6-1064">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="efdb6-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="efdb6-1065">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="efdb6-1066">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-1066">April 3, 2017</span></span>

<span data-ttu-id="efdb6-1067">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="efdb6-1067">Version 2.0.2</span></span>

<span data-ttu-id="efdb6-1068">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="efdb6-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```
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

### <a name="core"></a><span data-ttu-id="efdb6-1069">Principal</span><span class="sxs-lookup"><span data-stu-id="efdb6-1069">Core</span></span>

* <span data-ttu-id="efdb6-1070">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="efdb6-1071">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="efdb6-1072">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="efdb6-1073">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="efdb6-1074">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="efdb6-1075">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="efdb6-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="efdb6-1077">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="efdb6-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="efdb6-1078">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="efdb6-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="efdb6-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="efdb6-1079">ACS</span></span>

* <span data-ttu-id="efdb6-1080">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="efdb6-1081">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="efdb6-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="efdb6-1083">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1083">Add support for windows clusters.</span></span> <span data-ttu-id="efdb6-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="efdb6-1085">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="efdb6-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="efdb6-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="efdb6-1087">AppService</span></span>

* <span data-ttu-id="efdb6-1088">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="efdb6-1089">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="efdb6-1090">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="efdb6-1091">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="efdb6-1092">DataLake</span><span class="sxs-lookup"><span data-stu-id="efdb6-1092">DataLake</span></span>

* <span data-ttu-id="efdb6-1093">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="efdb6-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="efdb6-1094">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="efdb6-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="efdb6-1095">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="efdb6-1095">DocuemntDB</span></span>

* <span data-ttu-id="efdb6-1096">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="efdb6-1097">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="efdb6-1097">VM</span></span>

* <span data-ttu-id="efdb6-1098">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="efdb6-1099">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="efdb6-1100">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="efdb6-1101">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="efdb6-1102">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="efdb6-1103">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="efdb6-1104">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="efdb6-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="efdb6-1105">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="efdb6-1105">February 27, 2017</span></span>

<span data-ttu-id="efdb6-1106">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="efdb6-1106">Version 2.0.0</span></span>

<span data-ttu-id="efdb6-1107">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="efdb6-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="efdb6-1108">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="efdb6-1108">Container Service (acs)</span></span>
- <span data-ttu-id="efdb6-1109">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="efdb6-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="efdb6-1110">Réseau</span><span class="sxs-lookup"><span data-stu-id="efdb6-1110">Networking</span></span>
- <span data-ttu-id="efdb6-1111">Stockage</span><span class="sxs-lookup"><span data-stu-id="efdb6-1111">Storage</span></span>

<span data-ttu-id="efdb6-1112">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="efdb6-1113">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="efdb6-1114">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```
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
> <span data-ttu-id="efdb6-1115">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="efdb6-1116">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="efdb6-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="efdb6-1117">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="efdb6-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="efdb6-1118">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="efdb6-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="efdb6-1119">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="efdb6-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="efdb6-1120">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="efdb6-1120">Provide feedback from the command line with the `az feedback` command</span></span>

