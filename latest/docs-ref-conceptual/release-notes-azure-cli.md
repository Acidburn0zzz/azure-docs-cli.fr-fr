---
title: "Notes de publication d’Azure CLI 2.0"
description: "En savoir plus sur les dernières mises à jour d’Azure CLI 2.0"
keywords: Azure CLI 2.0, notes de publication
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="c6f7b-104">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c6f7b-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="c6f7b-105">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-105">October 9, 2017</span></span>

<span data-ttu-id="c6f7b-106">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c6f7b-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c6f7b-107">Principal</span><span class="sxs-lookup"><span data-stu-id="c6f7b-107">Core</span></span>

* <span data-ttu-id="c6f7b-108">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c6f7b-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-109">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-109">Appservice</span></span>

* <span data-ttu-id="c6f7b-110">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c6f7b-111">Batch</span><span class="sxs-lookup"><span data-stu-id="c6f7b-111">Batch</span></span>

* <span data-ttu-id="c6f7b-112">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c6f7b-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c6f7b-113">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="c6f7b-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c6f7b-114">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="c6f7b-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c6f7b-115">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="c6f7b-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c6f7b-116">Batchai</span><span class="sxs-lookup"><span data-stu-id="c6f7b-116">Batchai</span></span>

* <span data-ttu-id="c6f7b-117">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="c6f7b-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6f7b-118">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6f7b-118">Keyvault</span></span>

* <span data-ttu-id="c6f7b-119">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c6f7b-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c6f7b-121">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-121">Network</span></span>

* <span data-ttu-id="c6f7b-122">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="c6f7b-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c6f7b-123">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c6f7b-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c6f7b-124">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6f7b-124">Resource</span></span>

* <span data-ttu-id="c6f7b-125">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c6f7b-126">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c6f7b-127">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="c6f7b-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c6f7b-128">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c6f7b-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c6f7b-129">SQL</span><span class="sxs-lookup"><span data-stu-id="c6f7b-129">Sql</span></span>

* <span data-ttu-id="c6f7b-130">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="c6f7b-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c6f7b-131">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="c6f7b-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c6f7b-132">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="c6f7b-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-133">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-133">Storage</span></span>

* <span data-ttu-id="c6f7b-134">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="c6f7b-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-135">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-135">Vm</span></span>

* <span data-ttu-id="c6f7b-136">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="c6f7b-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c6f7b-137">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c6f7b-138">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c6f7b-139">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c6f7b-140">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c6f7b-141">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-141">September 22, 2017</span></span>

<span data-ttu-id="c6f7b-142">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c6f7b-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c6f7b-143">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6f7b-143">Resource</span></span>

* <span data-ttu-id="c6f7b-144">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c6f7b-145">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="c6f7b-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c6f7b-146">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c6f7b-147">[CHANGEMENT RÉCENT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-148">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-148">Network</span></span>

* <span data-ttu-id="c6f7b-149">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c6f7b-150">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c6f7b-151">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c6f7b-152">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c6f7b-153">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c6f7b-154">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c6f7b-155">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-156">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-156">Storage</span></span>

* <span data-ttu-id="c6f7b-157">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c6f7b-158">Événement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-158">Eventgrid</span></span>

* <span data-ttu-id="c6f7b-159">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="c6f7b-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c6f7b-160">SQL</span><span class="sxs-lookup"><span data-stu-id="c6f7b-160">SQL</span></span>

* <span data-ttu-id="c6f7b-161">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c6f7b-162">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c6f7b-163">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6f7b-164">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6f7b-164">Keyvault</span></span>

* <span data-ttu-id="c6f7b-165">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="c6f7b-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-166">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-166">VM</span></span>

* <span data-ttu-id="c6f7b-167">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c6f7b-168">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="c6f7b-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c6f7b-169">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c6f7b-170">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c6f7b-171">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c6f7b-172">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-173">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-173">ACS</span></span>

* <span data-ttu-id="c6f7b-174">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="c6f7b-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-175">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-175">Appservice</span></span>

* <span data-ttu-id="c6f7b-176">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c6f7b-177">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c6f7b-177">Backup</span></span>

* <span data-ttu-id="c6f7b-178">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c6f7b-179">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-179">September 11, 2017</span></span>

<span data-ttu-id="c6f7b-180">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c6f7b-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c6f7b-181">Principal</span><span class="sxs-lookup"><span data-stu-id="c6f7b-181">Core</span></span>

* <span data-ttu-id="c6f7b-182">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="c6f7b-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c6f7b-183">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="c6f7b-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-184">Acs</span><span class="sxs-lookup"><span data-stu-id="c6f7b-184">Acs</span></span>

* <span data-ttu-id="c6f7b-185">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c6f7b-186">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="c6f7b-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-187">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-187">Appservice</span></span>

* <span data-ttu-id="c6f7b-188">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="c6f7b-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c6f7b-189">CDN</span><span class="sxs-lookup"><span data-stu-id="c6f7b-189">CDN</span></span>

* <span data-ttu-id="c6f7b-190">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="c6f7b-191">Extension</span><span class="sxs-lookup"><span data-stu-id="c6f7b-191">Extension</span></span>

* <span data-ttu-id="c6f7b-192">Version initiale.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6f7b-193">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6f7b-193">Keyvault</span></span>

* <span data-ttu-id="c6f7b-194">Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-195">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-195">Network</span></span>

* <span data-ttu-id="c6f7b-196">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c6f7b-197">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c6f7b-198">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c6f7b-199">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c6f7b-200">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c6f7b-201">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6f7b-201">Resource</span></span>

* <span data-ttu-id="c6f7b-202">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c6f7b-203">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c6f7b-204">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="c6f7b-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c6f7b-205">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="c6f7b-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c6f7b-206">SQL</span><span class="sxs-lookup"><span data-stu-id="c6f7b-206">SQL</span></span>

* <span data-ttu-id="c6f7b-207">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-208">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-208">VM</span></span>

* <span data-ttu-id="c6f7b-209">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="c6f7b-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c6f7b-210">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="c6f7b-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c6f7b-211">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c6f7b-212">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="c6f7b-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c6f7b-213">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="c6f7b-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c6f7b-214">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-214">August 31, 2017</span></span>

<span data-ttu-id="c6f7b-215">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c6f7b-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6f7b-216">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6f7b-216">Keyvault</span></span>

* <span data-ttu-id="c6f7b-217">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c6f7b-218">Sf</span><span class="sxs-lookup"><span data-stu-id="c6f7b-218">Sf</span></span>

* <span data-ttu-id="c6f7b-219">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-220">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-220">Storage</span></span>

* <span data-ttu-id="c6f7b-221">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="c6f7b-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c6f7b-222">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c6f7b-223">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-223">August 28, 2017</span></span>

<span data-ttu-id="c6f7b-224">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c6f7b-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c6f7b-225">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c6f7b-225">CLI</span></span>

* <span data-ttu-id="c6f7b-226">Ajout d’une remarque juridique pour `--version`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-227">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-227">ACS</span></span>

* <span data-ttu-id="c6f7b-228">Correction des régions d’aperçu.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-228">Corrected preview regions.</span></span>
* <span data-ttu-id="c6f7b-229">Mise en forme par défaut `dns_name_prefix` correctement.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="c6f7b-230">Sortie de commande des services ACS optimisée.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-231">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-231">Appservice</span></span>

* <span data-ttu-id="c6f7b-232">[MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c6f7b-233">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c6f7b-234">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c6f7b-235">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c6f7b-236">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c6f7b-237">IoT</span><span class="sxs-lookup"><span data-stu-id="c6f7b-237">IoT</span></span>

* <span data-ttu-id="c6f7b-238">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="c6f7b-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-239">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-239">Network</span></span>

* <span data-ttu-id="c6f7b-240">[MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c6f7b-241">[MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c6f7b-242">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c6f7b-243">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c6f7b-244">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c6f7b-245">Profil</span><span class="sxs-lookup"><span data-stu-id="c6f7b-245">Profile</span></span>

* <span data-ttu-id="c6f7b-246">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c6f7b-247">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c6f7b-247">Service Fabric</span></span>

* <span data-ttu-id="c6f7b-248">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-248">Preview release</span></span>
* <span data-ttu-id="c6f7b-249">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="c6f7b-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c6f7b-250">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="c6f7b-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c6f7b-251">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-252">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-252">Storage</span></span>

* <span data-ttu-id="c6f7b-253">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="c6f7b-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="c6f7b-254">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="c6f7b-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c6f7b-255">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="c6f7b-256">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="c6f7b-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c6f7b-257">[MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande</span><span class="sxs-lookup"><span data-stu-id="c6f7b-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c6f7b-258">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="c6f7b-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-259">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-259">VM</span></span>

* <span data-ttu-id="c6f7b-260">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c6f7b-261">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c6f7b-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="c6f7b-262">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="c6f7b-263">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="c6f7b-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c6f7b-264">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="c6f7b-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c6f7b-265">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c6f7b-266">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-266">August 15, 2017</span></span>

<span data-ttu-id="c6f7b-267">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c6f7b-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-268">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-268">ACS</span></span>

* <span data-ttu-id="c6f7b-269">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="c6f7b-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-270">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-270">Appservice</span></span>

* <span data-ttu-id="c6f7b-271">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="c6f7b-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c6f7b-272">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c6f7b-272">Event Grid</span></span>

* <span data-ttu-id="c6f7b-273">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c6f7b-274">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-274">August 11, 2017</span></span>

<span data-ttu-id="c6f7b-275">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c6f7b-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-276">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-276">ACS</span></span>

* <span data-ttu-id="c6f7b-277">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c6f7b-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c6f7b-278">Batch</span><span class="sxs-lookup"><span data-stu-id="c6f7b-278">Batch</span></span>

* <span data-ttu-id="c6f7b-279">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c6f7b-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c6f7b-280">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="c6f7b-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c6f7b-281">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="c6f7b-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c6f7b-282">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="c6f7b-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c6f7b-283">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="c6f7b-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c6f7b-284">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="c6f7b-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c6f7b-285">Composant</span><span class="sxs-lookup"><span data-stu-id="c6f7b-285">Component</span></span>

* <span data-ttu-id="c6f7b-286">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="c6f7b-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c6f7b-287">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c6f7b-287">Container</span></span>

* <span data-ttu-id="c6f7b-288">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c6f7b-289">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c6f7b-289">Data Lake Store</span></span>

* <span data-ttu-id="c6f7b-290">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="c6f7b-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c6f7b-291">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c6f7b-291">Event Grid</span></span>

* <span data-ttu-id="c6f7b-292">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c6f7b-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-293">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-293">Network</span></span>

* <span data-ttu-id="c6f7b-294">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="c6f7b-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c6f7b-295">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c6f7b-296">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="c6f7b-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c6f7b-297">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c6f7b-298">Profil</span><span class="sxs-lookup"><span data-stu-id="c6f7b-298">Profile</span></span>

* <span data-ttu-id="c6f7b-299">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="c6f7b-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-300">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-300">Storage</span></span>

* <span data-ttu-id="c6f7b-301">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c6f7b-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-302">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-302">VM</span></span>

* <span data-ttu-id="c6f7b-303">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="c6f7b-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c6f7b-304">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c6f7b-305">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c6f7b-306">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="c6f7b-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c6f7b-307">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c6f7b-308">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-308">July 28, 2017</span></span>

<span data-ttu-id="c6f7b-309">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c6f7b-309">Version 2.0.12</span></span>

* <span data-ttu-id="c6f7b-310">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="c6f7b-310">Added container commands</span></span>
* <span data-ttu-id="c6f7b-311">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="c6f7b-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c6f7b-312">Principal</span><span class="sxs-lookup"><span data-stu-id="c6f7b-312">Core</span></span>

* <span data-ttu-id="c6f7b-313">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="c6f7b-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c6f7b-314">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c6f7b-315">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c6f7b-316">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c6f7b-317">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="c6f7b-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c6f7b-318">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c6f7b-319">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c6f7b-320">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c6f7b-321">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c6f7b-322">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c6f7b-323">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="c6f7b-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c6f7b-324">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c6f7b-325">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c6f7b-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c6f7b-326">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c6f7b-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c6f7b-327">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c6f7b-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c6f7b-328">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c6f7b-329">ACR</span><span class="sxs-lookup"><span data-stu-id="c6f7b-329">ACR</span></span>

* <span data-ttu-id="c6f7b-330">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c6f7b-331">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c6f7b-332">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c6f7b-333">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="c6f7b-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c6f7b-334">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="c6f7b-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c6f7b-335">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="c6f7b-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-336">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-336">ACS</span></span>

* <span data-ttu-id="c6f7b-337">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c6f7b-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-338">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-338">Appservice</span></span>

* <span data-ttu-id="c6f7b-339">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="c6f7b-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c6f7b-340">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="c6f7b-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c6f7b-341">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c6f7b-342">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c6f7b-343">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c6f7b-344">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c6f7b-345">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c6f7b-346">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c6f7b-347">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c6f7b-348">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c6f7b-349">Batch</span><span class="sxs-lookup"><span data-stu-id="c6f7b-349">Batch</span></span>

* <span data-ttu-id="c6f7b-350">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="c6f7b-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c6f7b-351">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c6f7b-352">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c6f7b-353">CDN</span><span class="sxs-lookup"><span data-stu-id="c6f7b-353">CDN</span></span>

* <span data-ttu-id="c6f7b-354">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="c6f7b-355">Cloud</span><span class="sxs-lookup"><span data-stu-id="c6f7b-355">Cloud</span></span>

* <span data-ttu-id="c6f7b-356">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="c6f7b-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c6f7b-357">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c6f7b-358">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="c6f7b-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c6f7b-359">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="c6f7b-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c6f7b-360">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c6f7b-361">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c6f7b-361">CosmosDB</span></span>

* <span data-ttu-id="c6f7b-362">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c6f7b-363">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c6f7b-364">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c6f7b-364">Data Lake Analytics</span></span>

* <span data-ttu-id="c6f7b-365">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c6f7b-366">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c6f7b-367">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c6f7b-368">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c6f7b-368">Data Lake Store</span></span>

* <span data-ttu-id="c6f7b-369">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c6f7b-370">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="c6f7b-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c6f7b-371">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c6f7b-372">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c6f7b-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c6f7b-373">Interactive</span><span class="sxs-lookup"><span data-stu-id="c6f7b-373">Interactive</span></span>

* <span data-ttu-id="c6f7b-374">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="c6f7b-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c6f7b-375">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="c6f7b-375">Increased test coverage</span></span>
* <span data-ttu-id="c6f7b-376">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="c6f7b-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c6f7b-377">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c6f7b-378">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c6f7b-379">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c6f7b-380">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c6f7b-381">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-381">Added `--progress` flag</span></span>
* <span data-ttu-id="c6f7b-382">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="c6f7b-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c6f7b-383">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c6f7b-384">IoT</span><span class="sxs-lookup"><span data-stu-id="c6f7b-384">IoT</span></span>

* <span data-ttu-id="c6f7b-385">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c6f7b-386">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c6f7b-387">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-387">Key vault</span></span>

* <span data-ttu-id="c6f7b-388">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c6f7b-389">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c6f7b-390">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c6f7b-391">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c6f7b-392">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c6f7b-393">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c6f7b-394">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c6f7b-395">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c6f7b-396">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-396">Lab</span></span>

* <span data-ttu-id="c6f7b-397">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c6f7b-398">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c6f7b-399">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c6f7b-399">Monitor</span></span>

* <span data-ttu-id="c6f7b-400">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c6f7b-401">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c6f7b-402">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c6f7b-403">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c6f7b-404">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c6f7b-405">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c6f7b-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c6f7b-406">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="c6f7b-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c6f7b-407">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c6f7b-408">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-408">`location` no longer required</span></span>
  * <span data-ttu-id="c6f7b-409">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="c6f7b-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="c6f7b-410">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c6f7b-411">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c6f7b-412">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="c6f7b-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c6f7b-413">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="c6f7b-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c6f7b-414">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c6f7b-415">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-416">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-416">Network</span></span>

* <span data-ttu-id="c6f7b-417">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c6f7b-418">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c6f7b-419">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="c6f7b-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c6f7b-420">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="c6f7b-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c6f7b-421">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c6f7b-422">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c6f7b-423">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c6f7b-424">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c6f7b-425">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c6f7b-426">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c6f7b-427">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c6f7b-428">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c6f7b-429">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c6f7b-430">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c6f7b-431">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c6f7b-432">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c6f7b-433">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c6f7b-434">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c6f7b-435">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c6f7b-436">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c6f7b-437">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c6f7b-438">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c6f7b-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c6f7b-439">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c6f7b-440">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c6f7b-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c6f7b-441">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c6f7b-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c6f7b-442">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c6f7b-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c6f7b-443">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c6f7b-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c6f7b-444">Profil</span><span class="sxs-lookup"><span data-stu-id="c6f7b-444">Profile</span></span>

* <span data-ttu-id="c6f7b-445">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="c6f7b-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c6f7b-446">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c6f7b-447">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="c6f7b-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c6f7b-448">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="c6f7b-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c6f7b-449">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="c6f7b-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c6f7b-450">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c6f7b-450">RDBMS</span></span>

* <span data-ttu-id="c6f7b-451">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c6f7b-452">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c6f7b-453">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c6f7b-454">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c6f7b-455">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6f7b-455">Resource</span></span>

* <span data-ttu-id="c6f7b-456">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c6f7b-457">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c6f7b-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c6f7b-458">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c6f7b-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c6f7b-459">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="c6f7b-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c6f7b-460">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c6f7b-461">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c6f7b-462">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c6f7b-463">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c6f7b-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c6f7b-464">Rôle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-464">Role</span></span>

* <span data-ttu-id="c6f7b-465">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c6f7b-466">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c6f7b-467">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="c6f7b-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c6f7b-468">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c6f7b-469">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c6f7b-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c6f7b-470">Service Fabric</span></span>
* <span data-ttu-id="c6f7b-471">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c6f7b-472">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c6f7b-473">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c6f7b-474">SQL</span><span class="sxs-lookup"><span data-stu-id="c6f7b-474">SQL</span></span>

* <span data-ttu-id="c6f7b-475">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c6f7b-476">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c6f7b-477">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-478">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-478">Storage</span></span>

* <span data-ttu-id="c6f7b-479">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c6f7b-480">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="c6f7b-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c6f7b-481">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c6f7b-482">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="c6f7b-483">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="c6f7b-484">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-485">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-485">VM</span></span>

* <span data-ttu-id="c6f7b-486">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-486">Support configuring nsg</span></span>
* <span data-ttu-id="c6f7b-487">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c6f7b-488">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="c6f7b-488">Support managed service identities</span></span>
* <span data-ttu-id="c6f7b-489">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="c6f7b-490">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="c6f7b-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c6f7b-491">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-491">May 10, 2017</span></span>

<span data-ttu-id="c6f7b-492">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c6f7b-492">Version 2.0.6</span></span>

* <span data-ttu-id="c6f7b-493">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c6f7b-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c6f7b-494">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c6f7b-495">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="c6f7b-496">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="c6f7b-497">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="c6f7b-498">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="c6f7b-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="c6f7b-499">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="c6f7b-500">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-500">Remove Container module.</span></span>
* <span data-ttu-id="c6f7b-501">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c6f7b-502">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c6f7b-503">Principal</span><span class="sxs-lookup"><span data-stu-id="c6f7b-503">Core</span></span>

* <span data-ttu-id="c6f7b-504">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="c6f7b-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="c6f7b-505">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c6f7b-506">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c6f7b-507">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c6f7b-508">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c6f7b-509">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c6f7b-510">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c6f7b-511">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c6f7b-512">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c6f7b-513">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="c6f7b-513">core: Improved performance</span></span>
* <span data-ttu-id="c6f7b-514">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c6f7b-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c6f7b-515">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="c6f7b-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c6f7b-516">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-516">ACS</span></span>

* <span data-ttu-id="c6f7b-517">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c6f7b-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c6f7b-518">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="c6f7b-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c6f7b-519">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="c6f7b-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c6f7b-520">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c6f7b-521">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-521">AppService</span></span>

* <span data-ttu-id="c6f7b-522">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c6f7b-523">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="c6f7b-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c6f7b-524">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c6f7b-525">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="c6f7b-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c6f7b-526">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="c6f7b-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c6f7b-527">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c6f7b-528">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="c6f7b-528">support slot swap with preview</span></span>
* <span data-ttu-id="c6f7b-529">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c6f7b-530">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c6f7b-531">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c6f7b-531">CosmosDB</span></span>

* <span data-ttu-id="c6f7b-532">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="c6f7b-533">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="c6f7b-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c6f7b-534">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="c6f7b-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c6f7b-535">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c6f7b-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c6f7b-536">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c6f7b-536">Data Lake Analytics</span></span>

* <span data-ttu-id="c6f7b-537">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="c6f7b-538">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c6f7b-539">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c6f7b-540">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c6f7b-541">Table</span><span class="sxs-lookup"><span data-stu-id="c6f7b-541">Table</span></span>
  * <span data-ttu-id="c6f7b-542">Fonction table</span><span class="sxs-lookup"><span data-stu-id="c6f7b-542">Table valued function</span></span>
  * <span data-ttu-id="c6f7b-543">Affichage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-543">View</span></span>
  * <span data-ttu-id="c6f7b-544">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-544">Table Statistics.</span></span> <span data-ttu-id="c6f7b-545">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c6f7b-546">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c6f7b-546">Data Lake Store</span></span>

* <span data-ttu-id="c6f7b-547">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="c6f7b-548">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c6f7b-549">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-549">missed help for access show.</span></span> <span data-ttu-id="c6f7b-550">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-550">adding it.</span></span> <span data-ttu-id="c6f7b-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c6f7b-552">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c6f7b-552">Find</span></span>

* <span data-ttu-id="c6f7b-553">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="c6f7b-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c6f7b-554">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c6f7b-554">KeyVault</span></span>

* <span data-ttu-id="c6f7b-555">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="c6f7b-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c6f7b-556">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="c6f7b-557">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="c6f7b-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c6f7b-558">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="c6f7b-559">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c6f7b-560">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c6f7b-560">Lab</span></span>

* <span data-ttu-id="c6f7b-561">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="c6f7b-562">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="c6f7b-563">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="c6f7b-564">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="c6f7b-565">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="c6f7b-566">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c6f7b-566">Monitor</span></span>

* <span data-ttu-id="c6f7b-567">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c6f7b-568">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c6f7b-569">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-569">Network</span></span>

* <span data-ttu-id="c6f7b-570">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="c6f7b-571">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="c6f7b-572">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="c6f7b-573">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="c6f7b-574">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="c6f7b-575">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="c6f7b-576">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="c6f7b-577">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="c6f7b-578">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="c6f7b-579">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="c6f7b-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c6f7b-580">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="c6f7b-581">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c6f7b-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="c6f7b-582">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="c6f7b-583">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="c6f7b-584">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="c6f7b-585">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="c6f7b-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="c6f7b-586">Profil</span><span class="sxs-lookup"><span data-stu-id="c6f7b-586">Profile</span></span>

* <span data-ttu-id="c6f7b-587">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c6f7b-588">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c6f7b-589">Redis</span><span class="sxs-lookup"><span data-stu-id="c6f7b-589">Redis</span></span>

* <span data-ttu-id="c6f7b-590">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="c6f7b-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c6f7b-591">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="c6f7b-592">Ressource</span><span class="sxs-lookup"><span data-stu-id="c6f7b-592">Resource</span></span>

* <span data-ttu-id="c6f7b-593">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c6f7b-594">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c6f7b-595">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c6f7b-596">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c6f7b-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c6f7b-598">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-598">Add docs for az lock update.</span></span> <span data-ttu-id="c6f7b-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c6f7b-600">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c6f7b-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c6f7b-602">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c6f7b-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c6f7b-604">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c6f7b-605">Rôle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-605">Role</span></span>

* <span data-ttu-id="c6f7b-606">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c6f7b-607">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c6f7b-608">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c6f7b-609">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="c6f7b-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c6f7b-610">SQL</span><span class="sxs-lookup"><span data-stu-id="c6f7b-610">SQL</span></span>

* <span data-ttu-id="c6f7b-611">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="c6f7b-612">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c6f7b-613">Storage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-613">Storage</span></span>

* <span data-ttu-id="c6f7b-614">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="c6f7b-615">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c6f7b-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c6f7b-616">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="c6f7b-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="c6f7b-617">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="c6f7b-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-618">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-618">VM</span></span>

* <span data-ttu-id="c6f7b-619">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="c6f7b-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c6f7b-620">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c6f7b-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c6f7b-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c6f7b-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c6f7b-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c6f7b-623">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="c6f7b-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c6f7b-624">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="c6f7b-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c6f7b-625">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c6f7b-626">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-626">April 3, 2017</span></span>

<span data-ttu-id="c6f7b-627">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c6f7b-627">Version 2.0.2</span></span>

<span data-ttu-id="c6f7b-628">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="c6f7b-629">Principal</span><span class="sxs-lookup"><span data-stu-id="c6f7b-629">Core</span></span>

* <span data-ttu-id="c6f7b-630">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="c6f7b-631">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c6f7b-632">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c6f7b-633">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c6f7b-634">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c6f7b-635">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c6f7b-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c6f7b-637">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="c6f7b-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c6f7b-638">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="c6f7b-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="c6f7b-639">ACS</span><span class="sxs-lookup"><span data-stu-id="c6f7b-639">ACS</span></span>

* <span data-ttu-id="c6f7b-640">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c6f7b-641">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c6f7b-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c6f7b-643">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-643">Add support for windows clusters.</span></span> <span data-ttu-id="c6f7b-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c6f7b-645">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c6f7b-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="c6f7b-647">AppService</span><span class="sxs-lookup"><span data-stu-id="c6f7b-647">AppService</span></span>

* <span data-ttu-id="c6f7b-648">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c6f7b-649">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c6f7b-650">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c6f7b-651">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="c6f7b-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="c6f7b-652">DataLake</span></span>

* <span data-ttu-id="c6f7b-653">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="c6f7b-654">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="c6f7b-655">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c6f7b-655">DocuemntDB</span></span>

* <span data-ttu-id="c6f7b-656">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c6f7b-657">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c6f7b-657">VM</span></span>

* <span data-ttu-id="c6f7b-658">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c6f7b-659">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c6f7b-660">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c6f7b-661">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c6f7b-662">Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c6f7b-663">Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="c6f7b-664">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c6f7b-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c6f7b-665">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="c6f7b-665">February 27, 2017</span></span>

<span data-ttu-id="c6f7b-666">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c6f7b-666">Version 2.0.0</span></span>

<span data-ttu-id="c6f7b-667">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="c6f7b-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="c6f7b-668">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="c6f7b-669">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-669">Container Service (acs)</span></span>
- <span data-ttu-id="c6f7b-670">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c6f7b-671">Réseau</span><span class="sxs-lookup"><span data-stu-id="c6f7b-671">Networking</span></span>
- <span data-ttu-id="c6f7b-672">Stockage</span><span class="sxs-lookup"><span data-stu-id="c6f7b-672">Storage</span></span>

<span data-ttu-id="c6f7b-673">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="c6f7b-674">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="c6f7b-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="c6f7b-675">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="c6f7b-676">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="c6f7b-677">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="c6f7b-678">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="c6f7b-679">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="c6f7b-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="c6f7b-680">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="c6f7b-681">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="c6f7b-682">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c6f7b-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="c6f7b-683">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="c6f7b-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c6f7b-684">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c6f7b-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c6f7b-685">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c6f7b-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="c6f7b-686">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c6f7b-686">Provide feedback from the command line with the `az feedback` command.</span></span>

