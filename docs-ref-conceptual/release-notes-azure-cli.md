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
ms.openlocfilehash: 116fa95e51399b9b97c1b35c38445f30db7efc94
ms.sourcegitcommit: fefb5bb6a21cab30c44592c0577408a8d1a2ccc7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/17/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="fe0d0-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="fe0d0-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="fe0d0-104">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="fe0d0-104">March 13, 2018</span></span>

<span data-ttu-id="fe0d0-105">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="fe0d0-105">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="fe0d0-106">ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-106">ACR</span></span>

* <span data-ttu-id="fe0d0-107">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-107">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="fe0d0-108">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-108">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="fe0d0-109">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="fe0d0-109">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-110">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-110">ACS</span></span>

* <span data-ttu-id="fe0d0-111">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="fe0d0-111">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="fe0d0-112">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="fe0d0-112">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="fe0d0-113">Advisor</span><span class="sxs-lookup"><span data-stu-id="fe0d0-113">Advisor</span></span>

* <span data-ttu-id="fe0d0-114">[MODIFICATION CRITIQUE] Renommage `advisor configuration get` à `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-114">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="fe0d0-115">[MODIFICATION CRITIQUE] Renommage `advisor configuration set` à `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-115">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="fe0d0-116">[MODIFICATION CRITIQUE] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-116">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="fe0d0-117">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-117">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="fe0d0-118">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-118">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-119">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-119">Appservice</span></span>

* <span data-ttu-id="fe0d0-120">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="fe0d0-120">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="fe0d0-121">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-121">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="fe0d0-122">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-122">Eventhubs</span></span>

* <span data-ttu-id="fe0d0-123">Version initiale</span><span class="sxs-lookup"><span data-stu-id="fe0d0-123">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="fe0d0-124">Extension</span><span class="sxs-lookup"><span data-stu-id="fe0d0-124">Extension</span></span>

* <span data-ttu-id="fe0d0-125">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-125">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="fe0d0-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="fe0d0-126">Interactive</span></span>

* <span data-ttu-id="fe0d0-127">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="fe0d0-127">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="fe0d0-128">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-128">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="fe0d0-129">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="fe0d0-129">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="fe0d0-130">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="fe0d0-130">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-131">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-131">Monitor</span></span>

* <span data-ttu-id="fe0d0-132">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-132">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="fe0d0-133">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-133">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="fe0d0-134">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-134">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="fe0d0-135">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-135">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-136">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-136">Network</span></span>

* <span data-ttu-id="fe0d0-137">[MODIFICATION CRITIQUE] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-137">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="fe0d0-138">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-138">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="fe0d0-139">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-139">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="fe0d0-140">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-140">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-141">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-141">Profile</span></span>

* <span data-ttu-id="fe0d0-142">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-142">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="fe0d0-143">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-143">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fe0d0-144">SGBDR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-144">RDBMS</span></span>

* <span data-ttu-id="fe0d0-145">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="fe0d0-145">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="fe0d0-146">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fe0d0-146">Service Bus</span></span>

* <span data-ttu-id="fe0d0-147">Version initiale</span><span class="sxs-lookup"><span data-stu-id="fe0d0-147">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-148">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-148">Storage</span></span>

* <span data-ttu-id="fe0d0-149">Résolu [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-149">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds.</span></span>
* <span data-ttu-id="fe0d0-150">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="fe0d0-150">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-151">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-151">VM</span></span>

* <span data-ttu-id="fe0d0-152">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="fe0d0-152">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="fe0d0-153">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-153">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="fe0d0-154">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-154">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="fe0d0-155">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="fe0d0-155">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="fe0d0-156">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="fe0d0-156">February 27, 2018</span></span>

<span data-ttu-id="fe0d0-157">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="fe0d0-157">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-158">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-158">Core</span></span>

* <span data-ttu-id="fe0d0-159">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="fe0d0-159">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="fe0d0-160">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-160">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="fe0d0-161">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-161">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-162">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-162">ACS</span></span>

* <span data-ttu-id="fe0d0-163">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-163">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="fe0d0-164">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-164">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="fe0d0-165">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-165">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="fe0d0-166">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-166">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-167">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-167">Appservice</span></span>

* <span data-ttu-id="fe0d0-168">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-168">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="fe0d0-169">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="fe0d0-169">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fe0d0-170">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fe0d0-170">Cognitive Services</span></span>

* <span data-ttu-id="fe0d0-171">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fe0d0-171">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="fe0d0-172">Consommation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-172">Consumption</span></span>

* <span data-ttu-id="fe0d0-173">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="fe0d0-173">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="fe0d0-174">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-174">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-175">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-175">Container</span></span>

* <span data-ttu-id="fe0d0-176">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-176">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-177">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-177">Network</span></span>

* <span data-ttu-id="fe0d0-178">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-178">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-179">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-179">Resource</span></span>

* <span data-ttu-id="fe0d0-180">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="fe0d0-180">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-181">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-181">Role</span></span>

* <span data-ttu-id="fe0d0-182">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="fe0d0-182">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-183">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-183">SQL</span></span>

* <span data-ttu-id="fe0d0-184">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="fe0d0-184">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-185">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-185">Storage</span></span>

* <span data-ttu-id="fe0d0-186">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-186">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-187">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-187">VM</span></span>

* <span data-ttu-id="fe0d0-188">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="fe0d0-188">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="fe0d0-189">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="fe0d0-189">February 13, 2018</span></span>

<span data-ttu-id="fe0d0-190">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="fe0d0-190">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-191">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-191">Core</span></span>

* <span data-ttu-id="fe0d0-192">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-192">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-193">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-193">ACS</span></span>

* <span data-ttu-id="fe0d0-194">[CHANGEMENT] `aks get-versions` renommé en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="fe0d0-194">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="fe0d0-195">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-195">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="fe0d0-196">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-196">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="fe0d0-197">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-197">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="fe0d0-198">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-198">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="fe0d0-199">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-199">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="fe0d0-200">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-200">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="fe0d0-201">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-201">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-202">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-202">Appservice</span></span>

* <span data-ttu-id="fe0d0-203">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="fe0d0-203">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="fe0d0-204">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-204">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="fe0d0-205">CDN</span><span class="sxs-lookup"><span data-stu-id="fe0d0-205">CDN</span></span>

* <span data-ttu-id="fe0d0-206">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-206">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-207">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-207">Container</span></span>

* <span data-ttu-id="fe0d0-208">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="fe0d0-208">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="fe0d0-209">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-209">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fe0d0-210">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fe0d0-210">CosmosDB</span></span>

* <span data-ttu-id="fe0d0-211">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="fe0d0-211">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="fe0d0-212">Extension</span><span class="sxs-lookup"><span data-stu-id="fe0d0-212">Extension</span></span>

* <span data-ttu-id="fe0d0-213">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-213">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="fe0d0-214">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-214">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="fe0d0-215">Commentaires</span><span class="sxs-lookup"><span data-stu-id="fe0d0-215">Feedback</span></span>

* <span data-ttu-id="fe0d0-216">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="fe0d0-216">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="fe0d0-217">Interactive</span><span class="sxs-lookup"><span data-stu-id="fe0d0-217">Interactive</span></span>

* <span data-ttu-id="fe0d0-218">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="fe0d0-218">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="fe0d0-219">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="fe0d0-219">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="fe0d0-220">IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-220">IoT</span></span>

* <span data-ttu-id="fe0d0-221">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-221">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="fe0d0-222">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-222">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="fe0d0-223">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-223">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="fe0d0-224">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="fe0d0-224">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-225">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-225">Monitor</span></span>

* <span data-ttu-id="fe0d0-226">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-226">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-227">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-227">Network</span></span>

* <span data-ttu-id="fe0d0-228">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-228">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="fe0d0-229">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-229">Profile</span></span>

* <span data-ttu-id="fe0d0-230">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-230">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-231">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-231">Resource</span></span>

* <span data-ttu-id="fe0d0-232">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-232">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-233">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-233">Role</span></span>

* <span data-ttu-id="fe0d0-234">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-234">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-235">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-235">SQL</span></span>

* <span data-ttu-id="fe0d0-236">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-236">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="fe0d0-237">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-237">Added `sql db rename`</span></span>
* <span data-ttu-id="fe0d0-238">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="fe0d0-238">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-239">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-239">Storage</span></span>

* <span data-ttu-id="fe0d0-240">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="fe0d0-240">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-241">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-241">VM</span></span>

* <span data-ttu-id="fe0d0-242">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-242">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="fe0d0-243">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-243">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="fe0d0-244">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-244">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="fe0d0-245">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="fe0d0-245">January 31, 2018</span></span>

<span data-ttu-id="fe0d0-246">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="fe0d0-246">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-247">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-247">Core</span></span>

* <span data-ttu-id="fe0d0-248">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-248">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="fe0d0-249">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="fe0d0-249">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="fe0d0-250">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-250">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="fe0d0-251">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="fe0d0-251">Use `--verbose` to see</span></span>
* <span data-ttu-id="fe0d0-252">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="fe0d0-252">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-253">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-253">ACS</span></span>

* <span data-ttu-id="fe0d0-254">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-254">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="fe0d0-255">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-255">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-256">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-256">Appservice</span></span>

* <span data-ttu-id="fe0d0-257">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-257">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="fe0d0-258">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="fe0d0-258">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="fe0d0-259">CDN</span><span class="sxs-lookup"><span data-stu-id="fe0d0-259">CDN</span></span>

* <span data-ttu-id="fe0d0-260">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-260">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fe0d0-261">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fe0d0-261">CosmosDB</span></span>

* <span data-ttu-id="fe0d0-262">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-262">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="fe0d0-263">Interactive</span><span class="sxs-lookup"><span data-stu-id="fe0d0-263">Interactive</span></span>

* <span data-ttu-id="fe0d0-264">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="fe0d0-264">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-265">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-265">Network</span></span>

* <span data-ttu-id="fe0d0-266">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-266">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="fe0d0-267">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-267">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="fe0d0-268">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-268">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="fe0d0-269">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-269">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="fe0d0-270">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-270">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="fe0d0-271">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-271">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="fe0d0-272">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-272">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="fe0d0-273">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-273">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="fe0d0-274">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-274">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="fe0d0-275">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-275">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-276">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-276">Profile</span></span>

* <span data-ttu-id="fe0d0-277">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="fe0d0-277">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-278">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-278">Resource</span></span>

* <span data-ttu-id="fe0d0-279">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="fe0d0-279">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-280">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-280">Storage</span></span>

* <span data-ttu-id="fe0d0-281">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="fe0d0-281">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="fe0d0-282">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-282">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="fe0d0-283">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-283">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="fe0d0-284">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-284">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="fe0d0-285">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="fe0d0-285">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-286">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-286">VM</span></span>

* <span data-ttu-id="fe0d0-287">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="fe0d0-287">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="fe0d0-288">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-288">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="fe0d0-289">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="fe0d0-289">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="fe0d0-290">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-290">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="fe0d0-291">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="fe0d0-291">January 17, 2018</span></span>

<span data-ttu-id="fe0d0-292">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="fe0d0-292">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="fe0d0-293">ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-293">ACR</span></span>

* <span data-ttu-id="fe0d0-294">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="fe0d0-294">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="fe0d0-295">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="fe0d0-295">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-296">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-296">ACS</span></span>

* <span data-ttu-id="fe0d0-297">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-297">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="fe0d0-298">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="fe0d0-298">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-299">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-299">Appservice</span></span>

* <span data-ttu-id="fe0d0-300">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="fe0d0-300">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="fe0d0-301">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-301">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="fe0d0-302">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-302">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="fe0d0-303">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="fe0d0-303">Backup</span></span>

* <span data-ttu-id="fe0d0-304">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="fe0d0-304">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="fe0d0-305">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-305">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="fe0d0-306">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="fe0d0-306">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="fe0d0-307">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="fe0d0-307">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="fe0d0-308">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-308">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="fe0d0-309">Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-309">Batch</span></span>

* <span data-ttu-id="fe0d0-310">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="fe0d0-310">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="fe0d0-311">Cloud</span><span class="sxs-lookup"><span data-stu-id="fe0d0-311">Cloud</span></span>

* <span data-ttu-id="fe0d0-312">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="fe0d0-312">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="fe0d0-313">Consommation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-313">Consumption</span></span>

* <span data-ttu-id="fe0d0-314">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-314">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="fe0d0-315">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fe0d0-315">Event Grid</span></span>

* <span data-ttu-id="fe0d0-316">[MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-316">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fe0d0-317">[MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-317">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fe0d0-318">[MODIFICATION CRITIQUE] Suppression de la commande `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-318">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="fe0d0-319">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="fe0d0-319">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="fe0d0-320">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-320">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="fe0d0-321">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-321">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="fe0d0-322">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-322">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="fe0d0-323">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="fe0d0-323">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="fe0d0-324">Interactive</span><span class="sxs-lookup"><span data-stu-id="fe0d0-324">Interactive</span></span>

* <span data-ttu-id="fe0d0-325">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="fe0d0-325">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="fe0d0-326">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-326">Fixed errors on startup</span></span>
* <span data-ttu-id="fe0d0-327">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-327">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="fe0d0-328">IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-328">IoT</span></span>

* <span data-ttu-id="fe0d0-329">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="fe0d0-329">Added support for device provisioning service</span></span>
* <span data-ttu-id="fe0d0-330">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-330">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="fe0d0-331">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-331">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-332">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-332">Monitor</span></span>

* <span data-ttu-id="fe0d0-333">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-333">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="fe0d0-334">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-334">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="fe0d0-335">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="fe0d0-335">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-336">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-336">Network</span></span>

* <span data-ttu-id="fe0d0-337">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-337">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="fe0d0-338">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-338">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-339">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-339">Profile</span></span>

* <span data-ttu-id="fe0d0-340">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-340">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-341">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-341">Role</span></span>

* <span data-ttu-id="fe0d0-342">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="fe0d0-342">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fe0d0-343">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fe0d0-343">Service Fabric</span></span>

* <span data-ttu-id="fe0d0-344">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="fe0d0-344">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="fe0d0-345">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-345">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-346">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-346">VM</span></span>

* <span data-ttu-id="fe0d0-347">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-347">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="fe0d0-348">[MODIFICATION CRITIQUE] Modification de zone unique `vmss` par défaut en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-348">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="fe0d0-349">[MODIFICATION CRITIQUE] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-349">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="fe0d0-350">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-350">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="fe0d0-351">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="fe0d0-351">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="fe0d0-352">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-352">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="fe0d0-353">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-353">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="fe0d0-354">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-354">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="fe0d0-355">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-355">December 19, 2017</span></span>

<span data-ttu-id="fe0d0-356">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="fe0d0-356">Version 2.0.23</span></span>

* <span data-ttu-id="fe0d0-357">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-357">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-358">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-358">Container</span></span>

* <span data-ttu-id="fe0d0-359">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-359">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-360">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-360">Network</span></span>

* <span data-ttu-id="fe0d0-361">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-361">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="fe0d0-362">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-362">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-363">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-363">Storage</span></span>

* <span data-ttu-id="fe0d0-364">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="fe0d0-364">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-365">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-365">VM</span></span>

* <span data-ttu-id="fe0d0-366">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-366">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="fe0d0-367">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-367">December 5, 2017</span></span>

<span data-ttu-id="fe0d0-368">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="fe0d0-368">Version 2.0.22</span></span>

* <span data-ttu-id="fe0d0-369">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-369">Removed `az component` commands.</span></span> <span data-ttu-id="fe0d0-370">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="fe0d0-370">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-371">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-371">Core</span></span>
* <span data-ttu-id="fe0d0-372">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="fe0d0-372">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="fe0d0-373">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-373">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-374">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-374">ACS</span></span>

* <span data-ttu-id="fe0d0-375">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-375">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="fe0d0-376">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-376">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="fe0d0-377">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="fe0d0-377">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="fe0d0-378">Advisor</span><span class="sxs-lookup"><span data-stu-id="fe0d0-378">Advisor</span></span>

* <span data-ttu-id="fe0d0-379">Version initiale</span><span class="sxs-lookup"><span data-stu-id="fe0d0-379">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-380">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-380">Appservice</span></span>

* <span data-ttu-id="fe0d0-381">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-381">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="fe0d0-382">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-382">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="fe0d0-383">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-383">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="fe0d0-384">Consommation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-384">Consumption</span></span>

* <span data-ttu-id="fe0d0-385">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="fe0d0-385">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-386">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-386">Container</span></span>

* <span data-ttu-id="fe0d0-387">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-387">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-388">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-388">Monitor</span></span>

* <span data-ttu-id="fe0d0-389">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="fe0d0-389">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-390">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-390">Resource</span></span>

* <span data-ttu-id="fe0d0-391">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-391">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-392">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-392">Role</span></span>

* <span data-ttu-id="fe0d0-393">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-393">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="fe0d0-394">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-394">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="fe0d0-395">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-395">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-396">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-396">SQL</span></span>

* <span data-ttu-id="fe0d0-397">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-397">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="fe0d0-398">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-398">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-399">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-399">VM</span></span>

* <span data-ttu-id="fe0d0-400">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-400">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="fe0d0-401">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-401">November 14, 2017</span></span>

<span data-ttu-id="fe0d0-402">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="fe0d0-402">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="fe0d0-403">ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-403">ACR</span></span>

* <span data-ttu-id="fe0d0-404">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="fe0d0-404">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="fe0d0-405">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-405">ACS</span></span>

* <span data-ttu-id="fe0d0-406">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-406">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="fe0d0-407">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-407">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="fe0d0-408">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-408">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="fe0d0-409">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="fe0d0-409">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="fe0d0-410">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="fe0d0-410">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-411">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-411">Appservice</span></span>

* <span data-ttu-id="fe0d0-412">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="fe0d0-412">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="fe0d0-413">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-413">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="fe0d0-414">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-414">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="fe0d0-415">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-415">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="fe0d0-416">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="fe0d0-416">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="fe0d0-417">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-417">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="fe0d0-418">Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-418">Batch</span></span>

* <span data-ttu-id="fe0d0-419">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-419">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="fe0d0-420">Batchai</span><span class="sxs-lookup"><span data-stu-id="fe0d0-420">Batchai</span></span>

* <span data-ttu-id="fe0d0-421">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-421">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="fe0d0-422">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-422">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="fe0d0-423">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-423">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="fe0d0-424">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-424">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="fe0d0-425">Cloud</span><span class="sxs-lookup"><span data-stu-id="fe0d0-425">Cloud</span></span>

* <span data-ttu-id="fe0d0-426">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="fe0d0-426">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-427">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-427">Container</span></span>

* <span data-ttu-id="fe0d0-428">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="fe0d0-428">Added support to open multiple ports</span></span>
* <span data-ttu-id="fe0d0-429">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-429">Added container group restart policy</span></span>
* <span data-ttu-id="fe0d0-430">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="fe0d0-430">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="fe0d0-431">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="fe0d0-431">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fe0d0-432">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fe0d0-432">Data Lake Analytics</span></span>

* <span data-ttu-id="fe0d0-433">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="fe0d0-433">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fe0d0-434">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fe0d0-434">Data Lake Store</span></span>

* <span data-ttu-id="fe0d0-435">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="fe0d0-435">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="fe0d0-436">Extension</span><span class="sxs-lookup"><span data-stu-id="fe0d0-436">Extension</span></span>

* <span data-ttu-id="fe0d0-437">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="fe0d0-437">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="fe0d0-438">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="fe0d0-438">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="fe0d0-439">IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-439">IoT</span></span>

* <span data-ttu-id="fe0d0-440">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-440">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-441">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-441">Monitor</span></span>

* <span data-ttu-id="fe0d0-442">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-442">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-443">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-443">Network</span></span>

* <span data-ttu-id="fe0d0-444">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="fe0d0-444">Added support for CAA DNS records</span></span>
* <span data-ttu-id="fe0d0-445">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-445">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="fe0d0-446">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="fe0d0-446">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="fe0d0-447">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-447">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="fe0d0-448">Réservations</span><span class="sxs-lookup"><span data-stu-id="fe0d0-448">Reservations</span></span>

* <span data-ttu-id="fe0d0-449">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="fe0d0-449">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-450">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-450">Resource</span></span>

* <span data-ttu-id="fe0d0-451">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="fe0d0-451">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-452">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-452">SQL</span></span>

* <span data-ttu-id="fe0d0-453">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-453">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-454">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-454">Storage</span></span>

* <span data-ttu-id="fe0d0-455">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-455">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="fe0d0-456">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="fe0d0-456">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="fe0d0-457">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-457">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="fe0d0-458">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-458">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="fe0d0-459">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-459">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="fe0d0-460">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-460">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="fe0d0-461">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-461">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-462">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-462">VM</span></span>

* <span data-ttu-id="fe0d0-463">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-463">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="fe0d0-464">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-464">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="fe0d0-465">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="fe0d0-465">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="fe0d0-466">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-466">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="fe0d0-467">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-467">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="fe0d0-468">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-468">October 24, 2017</span></span>

<span data-ttu-id="fe0d0-469">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="fe0d0-469">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-470">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-470">Core</span></span>

* <span data-ttu-id="fe0d0-471">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-471">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="fe0d0-472">ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-472">ACR</span></span>

* <span data-ttu-id="fe0d0-473">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-473">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="fe0d0-474">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="fe0d0-474">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="fe0d0-475">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="fe0d0-475">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-476">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-476">ACS</span></span>

* <span data-ttu-id="fe0d0-477">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-477">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="fe0d0-478">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-478">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-479">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-479">Appservice</span></span>

* <span data-ttu-id="fe0d0-480">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="fe0d0-480">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="fe0d0-481">Composant</span><span class="sxs-lookup"><span data-stu-id="fe0d0-481">Component</span></span>

* <span data-ttu-id="fe0d0-482">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-482">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-483">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-483">Monitor</span></span>

* <span data-ttu-id="fe0d0-484">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-484">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-485">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-485">Resource</span></span>

* <span data-ttu-id="fe0d0-486">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-486">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="fe0d0-487">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-487">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-488">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-488">VM</span></span>

* <span data-ttu-id="fe0d0-489">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-489">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="fe0d0-490">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-490">October 9, 2017</span></span>

<span data-ttu-id="fe0d0-491">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="fe0d0-491">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-492">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-492">Core</span></span>

* <span data-ttu-id="fe0d0-493">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="fe0d0-493">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-494">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-494">Appservice</span></span>

* <span data-ttu-id="fe0d0-495">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-495">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="fe0d0-496">Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-496">Batch</span></span>

* <span data-ttu-id="fe0d0-497">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="fe0d0-497">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="fe0d0-498">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="fe0d0-498">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="fe0d0-499">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-499">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="fe0d0-500">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="fe0d0-500">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="fe0d0-501">Batchai</span><span class="sxs-lookup"><span data-stu-id="fe0d0-501">Batchai</span></span>

* <span data-ttu-id="fe0d0-502">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="fe0d0-502">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="fe0d0-503">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fe0d0-503">Keyvault</span></span>

* <span data-ttu-id="fe0d0-504">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-504">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="fe0d0-505">(#4448)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-505">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="fe0d0-506">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-506">Network</span></span>

* <span data-ttu-id="fe0d0-507">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="fe0d0-507">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="fe0d0-508">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-508">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-509">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-509">Resource</span></span>

* <span data-ttu-id="fe0d0-510">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-510">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="fe0d0-511">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-511">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="fe0d0-512">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-512">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="fe0d0-513">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="fe0d0-513">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-514">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-514">Sql</span></span>

* <span data-ttu-id="fe0d0-515">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="fe0d0-515">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="fe0d0-516">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-516">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="fe0d0-517">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="fe0d0-517">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-518">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-518">Storage</span></span>

* <span data-ttu-id="fe0d0-519">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="fe0d0-519">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-520">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-520">Vm</span></span>

* <span data-ttu-id="fe0d0-521">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-521">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="fe0d0-522">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-522">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="fe0d0-523">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-523">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="fe0d0-524">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-524">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="fe0d0-525">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-525">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="fe0d0-526">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-526">September 22, 2017</span></span>

<span data-ttu-id="fe0d0-527">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="fe0d0-527">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-528">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-528">Resource</span></span>

* <span data-ttu-id="fe0d0-529">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-529">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="fe0d0-530">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="fe0d0-530">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="fe0d0-531">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-531">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="fe0d0-532">[CHANGEMENT RÉCENT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-532">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-533">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-533">Network</span></span>

* <span data-ttu-id="fe0d0-534">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-534">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="fe0d0-535">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-535">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="fe0d0-536">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-536">Added `asg` application security group commands</span></span>
* <span data-ttu-id="fe0d0-537">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-537">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="fe0d0-538">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-538">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fe0d0-539">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-539">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="fe0d0-540">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-540">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-541">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-541">Storage</span></span>

* <span data-ttu-id="fe0d0-542">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-542">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fe0d0-543">Événement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-543">Eventgrid</span></span>

* <span data-ttu-id="fe0d0-544">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-544">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-545">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-545">SQL</span></span>

* <span data-ttu-id="fe0d0-546">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-546">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="fe0d0-547">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-547">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="fe0d0-548">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-548">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="fe0d0-549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fe0d0-549">Keyvault</span></span>

* <span data-ttu-id="fe0d0-550">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="fe0d0-550">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-551">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-551">VM</span></span>

* <span data-ttu-id="fe0d0-552">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-552">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="fe0d0-553">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="fe0d0-553">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="fe0d0-554">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-554">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="fe0d0-555">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-555">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="fe0d0-556">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-556">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="fe0d0-557">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-557">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-558">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-558">ACS</span></span>

* <span data-ttu-id="fe0d0-559">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="fe0d0-559">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-560">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-560">Appservice</span></span>

* <span data-ttu-id="fe0d0-561">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-561">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fe0d0-562">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="fe0d0-562">Backup</span></span>

* <span data-ttu-id="fe0d0-563">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-563">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="fe0d0-564">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-564">September 11, 2017</span></span>

<span data-ttu-id="fe0d0-565">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="fe0d0-565">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="fe0d0-566">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-566">Core</span></span>

* <span data-ttu-id="fe0d0-567">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="fe0d0-567">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="fe0d0-568">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="fe0d0-568">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-569">Acs</span><span class="sxs-lookup"><span data-stu-id="fe0d0-569">Acs</span></span>

* <span data-ttu-id="fe0d0-570">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-570">Added `acs list-locations` command</span></span>
* <span data-ttu-id="fe0d0-571">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="fe0d0-571">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-572">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-572">Appservice</span></span>

* <span data-ttu-id="fe0d0-573">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-573">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="fe0d0-574">CDN</span><span class="sxs-lookup"><span data-stu-id="fe0d0-574">CDN</span></span>

* <span data-ttu-id="fe0d0-575">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-575">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="fe0d0-576">Extension</span><span class="sxs-lookup"><span data-stu-id="fe0d0-576">Extension</span></span>

* <span data-ttu-id="fe0d0-577">Version initiale.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-577">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="fe0d0-578">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fe0d0-578">Keyvault</span></span>

* <span data-ttu-id="fe0d0-579">Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-579">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-580">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-580">Network</span></span>

* <span data-ttu-id="fe0d0-581">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-581">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fe0d0-582">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-582">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="fe0d0-583">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-583">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="fe0d0-584">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-584">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fe0d0-585">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-585">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-586">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-586">Resource</span></span>

* <span data-ttu-id="fe0d0-587">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-587">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="fe0d0-588">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-588">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="fe0d0-589">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="fe0d0-589">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="fe0d0-590">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="fe0d0-590">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-591">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-591">SQL</span></span>

* <span data-ttu-id="fe0d0-592">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-592">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-593">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-593">VM</span></span>

* <span data-ttu-id="fe0d0-594">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="fe0d0-594">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="fe0d0-595">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="fe0d0-595">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="fe0d0-596">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-596">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="fe0d0-597">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="fe0d0-597">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="fe0d0-598">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="fe0d0-598">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="fe0d0-599">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-599">August 31, 2017</span></span>

<span data-ttu-id="fe0d0-600">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="fe0d0-600">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="fe0d0-601">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fe0d0-601">Keyvault</span></span>

* <span data-ttu-id="fe0d0-602">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-602">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="fe0d0-603">Sf</span><span class="sxs-lookup"><span data-stu-id="fe0d0-603">Sf</span></span>

* <span data-ttu-id="fe0d0-604">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-604">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-605">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-605">Storage</span></span>

* <span data-ttu-id="fe0d0-606">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="fe0d0-606">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="fe0d0-607">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-607">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="fe0d0-608">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-608">August 28, 2017</span></span>

<span data-ttu-id="fe0d0-609">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="fe0d0-609">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="fe0d0-610">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="fe0d0-610">CLI</span></span>

* <span data-ttu-id="fe0d0-611">Ajout d’une remarque juridique pour `--version`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-611">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-612">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-612">ACS</span></span>

* <span data-ttu-id="fe0d0-613">Correction des régions d’aperçu.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-613">Corrected preview regions.</span></span>
* <span data-ttu-id="fe0d0-614">Mise en forme par défaut `dns_name_prefix` correctement.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-614">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="fe0d0-615">Sortie de commande des services ACS optimisée.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-615">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-616">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-616">Appservice</span></span>

* <span data-ttu-id="fe0d0-617">[MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-617">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="fe0d0-618">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-618">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="fe0d0-619">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-619">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="fe0d0-620">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-620">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="fe0d0-621">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-621">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="fe0d0-622">IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-622">IoT</span></span>

* <span data-ttu-id="fe0d0-623">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-623">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-624">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-624">Network</span></span>

* <span data-ttu-id="fe0d0-625">[MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-625">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fe0d0-626">[MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-626">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="fe0d0-627">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-627">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fe0d0-628">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-628">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fe0d0-629">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-629">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-630">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-630">Profile</span></span>

* <span data-ttu-id="fe0d0-631">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-631">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fe0d0-632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fe0d0-632">Service Fabric</span></span>

* <span data-ttu-id="fe0d0-633">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-633">Preview release</span></span>
* <span data-ttu-id="fe0d0-634">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="fe0d0-634">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="fe0d0-635">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="fe0d0-635">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="fe0d0-636">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-636">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-637">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-637">Storage</span></span>

* <span data-ttu-id="fe0d0-638">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="fe0d0-638">Enabled setting blob tier</span></span>
* <span data-ttu-id="fe0d0-639">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="fe0d0-639">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="fe0d0-640">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-640">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="fe0d0-641">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="fe0d0-641">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="fe0d0-642">[MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande</span><span class="sxs-lookup"><span data-stu-id="fe0d0-642">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="fe0d0-643">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-643">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-644">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-644">VM</span></span>

* <span data-ttu-id="fe0d0-645">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-645">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="fe0d0-646">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="fe0d0-646">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="fe0d0-647">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-647">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="fe0d0-648">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="fe0d0-648">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="fe0d0-649">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="fe0d0-649">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="fe0d0-650">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-650">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="fe0d0-651">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-651">August 15, 2017</span></span>

<span data-ttu-id="fe0d0-652">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="fe0d0-652">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-653">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-653">ACS</span></span>

* <span data-ttu-id="fe0d0-654">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-654">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-655">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-655">Appservice</span></span>

* <span data-ttu-id="fe0d0-656">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="fe0d0-656">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="fe0d0-657">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fe0d0-657">Event Grid</span></span>

* <span data-ttu-id="fe0d0-658">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-658">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="fe0d0-659">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-659">August 11, 2017</span></span>

<span data-ttu-id="fe0d0-660">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="fe0d0-660">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-661">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-661">ACS</span></span>

* <span data-ttu-id="fe0d0-662">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="fe0d0-662">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="fe0d0-663">Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-663">Batch</span></span>

* <span data-ttu-id="fe0d0-664">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="fe0d0-664">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="fe0d0-665">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="fe0d0-665">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="fe0d0-666">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="fe0d0-666">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="fe0d0-667">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-667">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="fe0d0-668">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="fe0d0-668">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="fe0d0-669">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="fe0d0-669">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="fe0d0-670">Composant</span><span class="sxs-lookup"><span data-stu-id="fe0d0-670">Component</span></span>

* <span data-ttu-id="fe0d0-671">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-671">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="fe0d0-672">Conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-672">Container</span></span>

* <span data-ttu-id="fe0d0-673">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-673">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="fe0d0-674">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fe0d0-674">Data Lake Store</span></span>

* <span data-ttu-id="fe0d0-675">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="fe0d0-675">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="fe0d0-676">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fe0d0-676">Event Grid</span></span>

* <span data-ttu-id="fe0d0-677">Version initiale</span><span class="sxs-lookup"><span data-stu-id="fe0d0-677">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-678">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-678">Network</span></span>

* <span data-ttu-id="fe0d0-679">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="fe0d0-679">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="fe0d0-680">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-680">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="fe0d0-681">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="fe0d0-681">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="fe0d0-682">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-682">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-683">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-683">Profile</span></span>

* <span data-ttu-id="fe0d0-684">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-684">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-685">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-685">Storage</span></span>

* <span data-ttu-id="fe0d0-686">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="fe0d0-686">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-687">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-687">VM</span></span>

* <span data-ttu-id="fe0d0-688">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="fe0d0-688">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="fe0d0-689">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-689">Exposed `list-skus` command</span></span>
* <span data-ttu-id="fe0d0-690">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-690">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="fe0d0-691">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="fe0d0-691">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="fe0d0-692">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-692">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="fe0d0-693">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-693">July 28, 2017</span></span>

<span data-ttu-id="fe0d0-694">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="fe0d0-694">Version 2.0.12</span></span>

* <span data-ttu-id="fe0d0-695">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="fe0d0-695">Added container commands</span></span>
* <span data-ttu-id="fe0d0-696">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="fe0d0-696">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="fe0d0-697">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-697">Core</span></span>

* <span data-ttu-id="fe0d0-698">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="fe0d0-698">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="fe0d0-699">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-699">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="fe0d0-700">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-700">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="fe0d0-701">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-701">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="fe0d0-702">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="fe0d0-702">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="fe0d0-703">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-703">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="fe0d0-704">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-704">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fe0d0-705">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-705">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="fe0d0-706">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-706">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="fe0d0-707">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-707">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="fe0d0-708">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="fe0d0-708">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="fe0d0-709">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-709">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="fe0d0-710">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="fe0d0-710">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="fe0d0-711">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="fe0d0-711">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="fe0d0-712">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="fe0d0-712">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="fe0d0-713">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-713">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="fe0d0-714">ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-714">ACR</span></span>

* <span data-ttu-id="fe0d0-715">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-715">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="fe0d0-716">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-716">Support SKU update for managed registries</span></span>
* <span data-ttu-id="fe0d0-717">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-717">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="fe0d0-718">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="fe0d0-718">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="fe0d0-719">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="fe0d0-719">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="fe0d0-720">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="fe0d0-720">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-721">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-721">ACS</span></span>

* <span data-ttu-id="fe0d0-722">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="fe0d0-722">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-723">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-723">Appservice</span></span>

* <span data-ttu-id="fe0d0-724">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="fe0d0-724">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="fe0d0-725">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-725">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="fe0d0-726">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-726">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="fe0d0-727">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-727">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="fe0d0-728">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-728">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="fe0d0-729">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-729">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="fe0d0-730">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-730">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="fe0d0-731">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-731">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="fe0d0-732">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-732">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="fe0d0-733">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-733">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="fe0d0-734">Batch</span><span class="sxs-lookup"><span data-stu-id="fe0d0-734">Batch</span></span>

* <span data-ttu-id="fe0d0-735">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="fe0d0-735">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="fe0d0-736">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-736">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="fe0d0-737">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-737">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="fe0d0-738">CDN</span><span class="sxs-lookup"><span data-stu-id="fe0d0-738">CDN</span></span>

* <span data-ttu-id="fe0d0-739">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-739">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="fe0d0-740">Cloud</span><span class="sxs-lookup"><span data-stu-id="fe0d0-740">Cloud</span></span>

* <span data-ttu-id="fe0d0-741">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="fe0d0-741">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="fe0d0-742">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-742">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="fe0d0-743">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="fe0d0-743">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="fe0d0-744">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="fe0d0-744">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="fe0d0-745">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-745">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fe0d0-746">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fe0d0-746">CosmosDB</span></span>

* <span data-ttu-id="fe0d0-747">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-747">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="fe0d0-748">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-748">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fe0d0-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fe0d0-749">Data Lake Analytics</span></span>

* <span data-ttu-id="fe0d0-750">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-750">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="fe0d0-751">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-751">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="fe0d0-752">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-752">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fe0d0-753">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fe0d0-753">Data Lake Store</span></span>

* <span data-ttu-id="fe0d0-754">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-754">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="fe0d0-755">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="fe0d0-755">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="fe0d0-756">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-756">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="fe0d0-757">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fe0d0-757">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="fe0d0-758">Interactive</span><span class="sxs-lookup"><span data-stu-id="fe0d0-758">Interactive</span></span>

* <span data-ttu-id="fe0d0-759">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="fe0d0-759">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="fe0d0-760">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="fe0d0-760">Increased test coverage</span></span>
* <span data-ttu-id="fe0d0-761">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="fe0d0-761">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="fe0d0-762">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-762">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="fe0d0-763">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-763">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="fe0d0-764">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-764">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="fe0d0-765">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-765">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fe0d0-766">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-766">Added `--progress` flag</span></span>
* <span data-ttu-id="fe0d0-767">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="fe0d0-767">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="fe0d0-768">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-768">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="fe0d0-769">IoT</span><span class="sxs-lookup"><span data-stu-id="fe0d0-769">IoT</span></span>

* <span data-ttu-id="fe0d0-770">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-770">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="fe0d0-771">(#3934)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-771">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="fe0d0-772">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-772">Key vault</span></span>

* <span data-ttu-id="fe0d0-773">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-773">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="fe0d0-774">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-774">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="fe0d0-775">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-775">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fe0d0-776">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-776">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fe0d0-777">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-777">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="fe0d0-778">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-778">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="fe0d0-779">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-779">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="fe0d0-780">(#3307)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-780">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="fe0d0-781">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-781">Lab</span></span>

* <span data-ttu-id="fe0d0-782">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-782">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="fe0d0-783">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-783">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-784">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-784">Monitor</span></span>

* <span data-ttu-id="fe0d0-785">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-785">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="fe0d0-786">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-786">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="fe0d0-787">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-787">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="fe0d0-788">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-788">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="fe0d0-789">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-789">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="fe0d0-790">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="fe0d0-790">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="fe0d0-791">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="fe0d0-791">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="fe0d0-792">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-792">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="fe0d0-793">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-793">`location` no longer required</span></span>
  * <span data-ttu-id="fe0d0-794">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="fe0d0-794">Add name and ID support for target</span></span>
  * <span data-ttu-id="fe0d0-795">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-795">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="fe0d0-796">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-796">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="fe0d0-797">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="fe0d0-797">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="fe0d0-798">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="fe0d0-798">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="fe0d0-799">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-799">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="fe0d0-800">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-800">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-801">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-801">Network</span></span>

* <span data-ttu-id="fe0d0-802">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-802">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="fe0d0-803">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-803">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="fe0d0-804">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="fe0d0-804">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="fe0d0-805">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="fe0d0-805">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="fe0d0-806">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-806">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="fe0d0-807">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-807">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="fe0d0-808">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-808">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="fe0d0-809">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-809">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="fe0d0-810">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-810">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="fe0d0-811">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-811">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="fe0d0-812">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-812">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="fe0d0-813">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-813">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="fe0d0-814">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-814">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="fe0d0-815">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-815">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="fe0d0-816">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-816">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="fe0d0-817">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-817">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="fe0d0-818">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-818">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="fe0d0-819">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-819">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="fe0d0-820">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-820">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="fe0d0-821">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-821">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="fe0d0-822">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-822">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="fe0d0-823">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-823">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="fe0d0-824">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-824">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="fe0d0-825">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="fe0d0-825">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="fe0d0-826">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="fe0d0-826">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="fe0d0-827">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="fe0d0-827">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="fe0d0-828">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="fe0d0-828">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-829">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-829">Profile</span></span>

* <span data-ttu-id="fe0d0-830">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="fe0d0-830">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="fe0d0-831">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-831">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="fe0d0-832">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="fe0d0-832">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="fe0d0-833">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-833">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="fe0d0-834">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="fe0d0-834">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="fe0d0-835">SGBDR</span><span class="sxs-lookup"><span data-stu-id="fe0d0-835">RDBMS</span></span>

* <span data-ttu-id="fe0d0-836">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-836">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="fe0d0-837">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-837">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="fe0d0-838">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-838">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="fe0d0-839">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-839">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-840">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-840">Resource</span></span>

* <span data-ttu-id="fe0d0-841">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-841">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="fe0d0-842">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-842">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="fe0d0-843">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-843">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="fe0d0-844">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="fe0d0-844">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="fe0d0-845">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-845">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="fe0d0-846">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-846">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="fe0d0-847">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-847">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="fe0d0-848">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="fe0d0-848">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-849">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-849">Role</span></span>

* <span data-ttu-id="fe0d0-850">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-850">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="fe0d0-851">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-851">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="fe0d0-852">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="fe0d0-852">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="fe0d0-853">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-853">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="fe0d0-854">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-854">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fe0d0-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fe0d0-855">Service Fabric</span></span>
* <span data-ttu-id="fe0d0-856">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-856">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="fe0d0-857">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-857">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="fe0d0-858">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-858">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-859">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-859">SQL</span></span>

* <span data-ttu-id="fe0d0-860">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-860">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="fe0d0-861">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-861">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="fe0d0-862">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-862">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-863">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-863">Storage</span></span>

* <span data-ttu-id="fe0d0-864">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-864">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="fe0d0-865">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="fe0d0-865">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="fe0d0-866">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-866">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="fe0d0-867">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-867">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="fe0d0-868">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-868">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="fe0d0-869">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-869">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-870">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-870">VM</span></span>

* <span data-ttu-id="fe0d0-871">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-871">Support configuring nsg</span></span>
* <span data-ttu-id="fe0d0-872">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-872">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="fe0d0-873">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="fe0d0-873">Support managed service identities</span></span>
* <span data-ttu-id="fe0d0-874">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-874">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="fe0d0-875">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="fe0d0-875">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="fe0d0-876">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-876">May 10, 2017</span></span>

<span data-ttu-id="fe0d0-877">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="fe0d0-877">Version 2.0.6</span></span>

* <span data-ttu-id="fe0d0-878">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="fe0d0-878">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="fe0d0-879">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-879">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="fe0d0-880">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-880">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="fe0d0-881">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-881">Include Cognitive Services module.</span></span>
* <span data-ttu-id="fe0d0-882">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-882">Include Service Fabric module.</span></span>
* <span data-ttu-id="fe0d0-883">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="fe0d0-883">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="fe0d0-884">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-884">Add support for CDN commands.</span></span>
* <span data-ttu-id="fe0d0-885">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-885">Remove Container module.</span></span>
* <span data-ttu-id="fe0d0-886">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-886">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="fe0d0-887">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-887">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="fe0d0-888">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-888">Core</span></span>

* <span data-ttu-id="fe0d0-889">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="fe0d0-889">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="fe0d0-890">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-890">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="fe0d0-891">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-891">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="fe0d0-892">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-892">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="fe0d0-893">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-893">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="fe0d0-894">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-894">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="fe0d0-895">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-895">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="fe0d0-896">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-896">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="fe0d0-897">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-897">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="fe0d0-898">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="fe0d0-898">core: Improved performance</span></span>
* <span data-ttu-id="fe0d0-899">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="fe0d0-899">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="fe0d0-900">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="fe0d0-900">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-901">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-901">ACS</span></span>

* <span data-ttu-id="fe0d0-902">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="fe0d0-902">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="fe0d0-903">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="fe0d0-903">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="fe0d0-904">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="fe0d0-904">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="fe0d0-905">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-905">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-906">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-906">AppService</span></span>

* <span data-ttu-id="fe0d0-907">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-907">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="fe0d0-908">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-908">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="fe0d0-909">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-909">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="fe0d0-910">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="fe0d0-910">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="fe0d0-911">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="fe0d0-911">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="fe0d0-912">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-912">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="fe0d0-913">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="fe0d0-913">support slot swap with preview</span></span>
* <span data-ttu-id="fe0d0-914">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-914">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="fe0d0-915">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-915">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fe0d0-916">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fe0d0-916">CosmosDB</span></span>

* <span data-ttu-id="fe0d0-917">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-917">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="fe0d0-918">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="fe0d0-918">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="fe0d0-919">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="fe0d0-919">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="fe0d0-920">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="fe0d0-920">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fe0d0-921">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fe0d0-921">Data Lake Analytics</span></span>

* <span data-ttu-id="fe0d0-922">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-922">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="fe0d0-923">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-923">Add support for new catalog item type: package.</span></span> <span data-ttu-id="fe0d0-924">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-924">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="fe0d0-925">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-925">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="fe0d0-926">Table</span><span class="sxs-lookup"><span data-stu-id="fe0d0-926">Table</span></span>
  * <span data-ttu-id="fe0d0-927">Fonction table</span><span class="sxs-lookup"><span data-stu-id="fe0d0-927">Table valued function</span></span>
  * <span data-ttu-id="fe0d0-928">Affichage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-928">View</span></span>
  * <span data-ttu-id="fe0d0-929">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-929">Table Statistics.</span></span> <span data-ttu-id="fe0d0-930">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-930">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fe0d0-931">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fe0d0-931">Data Lake Store</span></span>

* <span data-ttu-id="fe0d0-932">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-932">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="fe0d0-933">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-933">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="fe0d0-934">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-934">missed help for access show.</span></span> <span data-ttu-id="fe0d0-935">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-935">adding it.</span></span> <span data-ttu-id="fe0d0-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="fe0d0-937">Rechercher</span><span class="sxs-lookup"><span data-stu-id="fe0d0-937">Find</span></span>

* <span data-ttu-id="fe0d0-938">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="fe0d0-938">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="fe0d0-939">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fe0d0-939">KeyVault</span></span>

* <span data-ttu-id="fe0d0-940">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="fe0d0-940">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="fe0d0-941">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-941">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="fe0d0-942">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="fe0d0-942">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="fe0d0-943">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-943">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="fe0d0-944">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-944">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="fe0d0-945">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="fe0d0-945">Lab</span></span>

* <span data-ttu-id="fe0d0-946">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-946">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="fe0d0-947">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-947">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="fe0d0-948">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-948">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="fe0d0-949">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-949">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="fe0d0-950">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-950">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="fe0d0-951">Surveiller</span><span class="sxs-lookup"><span data-stu-id="fe0d0-951">Monitor</span></span>

* <span data-ttu-id="fe0d0-952">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-952">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="fe0d0-953">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-953">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="fe0d0-954">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-954">Network</span></span>

* <span data-ttu-id="fe0d0-955">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-955">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="fe0d0-956">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-956">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="fe0d0-957">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-957">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="fe0d0-958">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-958">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="fe0d0-959">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-959">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="fe0d0-960">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-960">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="fe0d0-961">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-961">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="fe0d0-962">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-962">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="fe0d0-963">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-963">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="fe0d0-964">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-964">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="fe0d0-965">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-965">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="fe0d0-966">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="fe0d0-966">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="fe0d0-967">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-967">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="fe0d0-968">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-968">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="fe0d0-969">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-969">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="fe0d0-970">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="fe0d0-970">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="fe0d0-971">Profil</span><span class="sxs-lookup"><span data-stu-id="fe0d0-971">Profile</span></span>

* <span data-ttu-id="fe0d0-972">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-972">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="fe0d0-973">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-973">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="fe0d0-974">Redis</span><span class="sxs-lookup"><span data-stu-id="fe0d0-974">Redis</span></span>

* <span data-ttu-id="fe0d0-975">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="fe0d0-975">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="fe0d0-976">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-976">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="fe0d0-977">Ressource</span><span class="sxs-lookup"><span data-stu-id="fe0d0-977">Resource</span></span>

* <span data-ttu-id="fe0d0-978">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-978">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="fe0d0-979">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-979">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="fe0d0-980">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-980">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="fe0d0-981">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-981">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="fe0d0-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="fe0d0-983">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-983">Add docs for az lock update.</span></span> <span data-ttu-id="fe0d0-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="fe0d0-985">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-985">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="fe0d0-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="fe0d0-987">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-987">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="fe0d0-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="fe0d0-989">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-989">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="fe0d0-990">Rôle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-990">Role</span></span>

* <span data-ttu-id="fe0d0-991">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-991">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="fe0d0-992">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-992">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="fe0d0-993">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-993">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="fe0d0-994">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="fe0d0-994">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="fe0d0-995">SQL</span><span class="sxs-lookup"><span data-stu-id="fe0d0-995">SQL</span></span>

* <span data-ttu-id="fe0d0-996">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-996">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="fe0d0-997">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-997">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="fe0d0-998">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-998">Storage</span></span>

* <span data-ttu-id="fe0d0-999">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-999">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="fe0d0-1000">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1000">Add support for incremental blob copy</span></span>
* <span data-ttu-id="fe0d0-1001">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1001">Add support for large block blob upload</span></span>
* <span data-ttu-id="fe0d0-1002">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1002">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-1003">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1003">VM</span></span>

* <span data-ttu-id="fe0d0-1004">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1004">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="fe0d0-1005">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1005">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="fe0d0-1006">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1006">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="fe0d0-1007">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1007">az vm/vmss disk</span></span>
  3. <span data-ttu-id="fe0d0-1008">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1008">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="fe0d0-1009">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1009">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="fe0d0-1010">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1010">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="fe0d0-1011">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1011">April 3, 2017</span></span>

<span data-ttu-id="fe0d0-1012">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1012">Version 2.0.2</span></span>

<span data-ttu-id="fe0d0-1013">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1013">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="fe0d0-1014">Principal</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1014">Core</span></span>

* <span data-ttu-id="fe0d0-1015">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1015">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="fe0d0-1016">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1016">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="fe0d0-1017">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1017">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="fe0d0-1018">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1018">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fe0d0-1019">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1019">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="fe0d0-1020">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1020">Add prompting for missing template parameters.</span></span> <span data-ttu-id="fe0d0-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="fe0d0-1022">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1022">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="fe0d0-1023">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1023">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="fe0d0-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1024">ACS</span></span>

* <span data-ttu-id="fe0d0-1025">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1025">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="fe0d0-1026">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1026">Add support for ssh key password prompting.</span></span> <span data-ttu-id="fe0d0-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="fe0d0-1028">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1028">Add support for windows clusters.</span></span> <span data-ttu-id="fe0d0-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="fe0d0-1030">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1030">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="fe0d0-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="fe0d0-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1032">AppService</span></span>

* <span data-ttu-id="fe0d0-1033">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1033">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="fe0d0-1034">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1034">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="fe0d0-1035">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1035">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="fe0d0-1036">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1036">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="fe0d0-1037">DataLake</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1037">DataLake</span></span>

* <span data-ttu-id="fe0d0-1038">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1038">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="fe0d0-1039">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1039">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="fe0d0-1040">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1040">DocuemntDB</span></span>

* <span data-ttu-id="fe0d0-1041">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1041">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="fe0d0-1042">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1042">VM</span></span>

* <span data-ttu-id="fe0d0-1043">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1043">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="fe0d0-1044">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1044">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="fe0d0-1045">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1045">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="fe0d0-1046">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1046">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fe0d0-1047">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1047">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="fe0d0-1048">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1048">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="fe0d0-1049">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1049">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="fe0d0-1050">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1050">February 27, 2017</span></span>

<span data-ttu-id="fe0d0-1051">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1051">Version 2.0.0</span></span>

<span data-ttu-id="fe0d0-1052">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1052">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="fe0d0-1053">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1053">General availability applies to these command modules:</span></span>
- <span data-ttu-id="fe0d0-1054">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1054">Container Service (acs)</span></span>
- <span data-ttu-id="fe0d0-1055">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1055">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="fe0d0-1056">Réseau</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1056">Networking</span></span>
- <span data-ttu-id="fe0d0-1057">Stockage</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1057">Storage</span></span>

<span data-ttu-id="fe0d0-1058">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1058">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="fe0d0-1059">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1059">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="fe0d0-1060">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1060">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="fe0d0-1061">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1061">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="fe0d0-1062">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1062">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="fe0d0-1063">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1063">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="fe0d0-1064">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1064">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="fe0d0-1065">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1065">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="fe0d0-1066">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1066">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="fe0d0-1067">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1067">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="fe0d0-1068">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1068">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="fe0d0-1069">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1069">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="fe0d0-1070">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1070">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="fe0d0-1071">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="fe0d0-1071">Provide feedback from the command line with the `az feedback` command.</span></span>

