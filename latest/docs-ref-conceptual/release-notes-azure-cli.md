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
ms.openlocfilehash: 761bd61474e7c72fb2daeb756828f00196b56c3a
ms.sourcegitcommit: bb649ebd7e7fce8fb5008ac1e2e2c33481a45df9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/16/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="1de5d-104">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="1de5d-104">Azure CLI 2.0 release notes</span></span>

## <a name="november-14-2017"></a><span data-ttu-id="1de5d-105">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-105">November 14, 2017</span></span>

<span data-ttu-id="1de5d-106">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1de5d-106">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1de5d-107">ACR</span><span class="sxs-lookup"><span data-stu-id="1de5d-107">ACR</span></span>

* <span data-ttu-id="1de5d-108">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="1de5d-108">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1de5d-109">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-109">ACS</span></span>

* <span data-ttu-id="1de5d-110">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="1de5d-110">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1de5d-111">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-111">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="1de5d-112">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="1de5d-112">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="1de5d-113">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1de5d-113">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1de5d-114">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="1de5d-114">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-115">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-115">Appservice</span></span>

* <span data-ttu-id="1de5d-116">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="1de5d-116">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1de5d-117">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1de5d-117">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="1de5d-118">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1de5d-118">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="1de5d-119">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="1de5d-119">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="1de5d-120">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="1de5d-120">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1de5d-121">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="1de5d-121">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="1de5d-122">Batch</span><span class="sxs-lookup"><span data-stu-id="1de5d-122">Batch</span></span>

* <span data-ttu-id="1de5d-123">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="1de5d-123">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1de5d-124">Batchai</span><span class="sxs-lookup"><span data-stu-id="1de5d-124">Batchai</span></span>

* <span data-ttu-id="1de5d-125">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-125">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1de5d-126">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-126">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1de5d-127">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="1de5d-127">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="1de5d-128">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-128">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1de5d-129">Cloud</span><span class="sxs-lookup"><span data-stu-id="1de5d-129">Cloud</span></span>

* <span data-ttu-id="1de5d-130">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="1de5d-130">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1de5d-131">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1de5d-131">Container</span></span>

* <span data-ttu-id="1de5d-132">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="1de5d-132">Added support to open multiple ports</span></span>
* <span data-ttu-id="1de5d-133">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="1de5d-133">Added container group restart policy</span></span>
* <span data-ttu-id="1de5d-134">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="1de5d-134">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1de5d-135">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="1de5d-135">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1de5d-136">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1de5d-136">Data Lake Analytics</span></span>

* <span data-ttu-id="1de5d-137">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="1de5d-137">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1de5d-138">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1de5d-138">Data Lake Store</span></span>

* <span data-ttu-id="1de5d-139">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="1de5d-139">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1de5d-140">Extension</span><span class="sxs-lookup"><span data-stu-id="1de5d-140">Extension</span></span>

* <span data-ttu-id="1de5d-141">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="1de5d-141">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1de5d-142">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="1de5d-142">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1de5d-143">IoT</span><span class="sxs-lookup"><span data-stu-id="1de5d-143">IoT</span></span>

* <span data-ttu-id="1de5d-144">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="1de5d-144">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1de5d-145">Surveiller</span><span class="sxs-lookup"><span data-stu-id="1de5d-145">Monitor</span></span>

* <span data-ttu-id="1de5d-146">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="1de5d-146">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-147">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-147">Network</span></span>

* <span data-ttu-id="1de5d-148">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="1de5d-148">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1de5d-149">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-149">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="1de5d-150">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="1de5d-150">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1de5d-151">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="1de5d-151">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="1de5d-152">Réservations</span><span class="sxs-lookup"><span data-stu-id="1de5d-152">Reservations</span></span>

* <span data-ttu-id="1de5d-153">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="1de5d-153">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-154">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-154">Resource</span></span>

* <span data-ttu-id="1de5d-155">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="1de5d-155">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-156">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-156">SQL</span></span>

* <span data-ttu-id="1de5d-157">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-157">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-158">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-158">Storage</span></span>

* <span data-ttu-id="1de5d-159">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="1de5d-159">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1de5d-160">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="1de5d-160">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1de5d-161">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="1de5d-161">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="1de5d-162">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="1de5d-162">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="1de5d-163">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-163">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="1de5d-164">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="1de5d-164">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="1de5d-165">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-165">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-166">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-166">VM</span></span>

* <span data-ttu-id="1de5d-167">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="1de5d-167">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1de5d-168">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="1de5d-168">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1de5d-169">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="1de5d-169">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1de5d-170">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="1de5d-170">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="1de5d-171">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1de5d-171">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="1de5d-172">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-172">October 24, 2017</span></span>

<span data-ttu-id="1de5d-173">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1de5d-173">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1de5d-174">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-174">Core</span></span>

* <span data-ttu-id="1de5d-175">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="1de5d-175">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="1de5d-176">ACR</span><span class="sxs-lookup"><span data-stu-id="1de5d-176">ACR</span></span>

* <span data-ttu-id="1de5d-177">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="1de5d-177">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1de5d-178">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="1de5d-178">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1de5d-179">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="1de5d-179">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-180">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-180">ACS</span></span>

* <span data-ttu-id="1de5d-181">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="1de5d-181">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1de5d-182">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1de5d-182">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-183">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-183">Appservice</span></span>

* <span data-ttu-id="1de5d-184">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="1de5d-184">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1de5d-185">Composant</span><span class="sxs-lookup"><span data-stu-id="1de5d-185">Component</span></span>

* <span data-ttu-id="1de5d-186">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="1de5d-186">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1de5d-187">Surveiller</span><span class="sxs-lookup"><span data-stu-id="1de5d-187">Monitor</span></span>

* <span data-ttu-id="1de5d-188">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="1de5d-188">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-189">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-189">Resource</span></span>

* <span data-ttu-id="1de5d-190">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="1de5d-190">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="1de5d-191">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="1de5d-191">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-192">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-192">VM</span></span>

* <span data-ttu-id="1de5d-193">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-193">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="1de5d-194">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-194">October 9, 2017</span></span>

<span data-ttu-id="1de5d-195">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1de5d-195">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1de5d-196">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-196">Core</span></span>

* <span data-ttu-id="1de5d-197">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1de5d-197">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-198">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-198">Appservice</span></span>

* <span data-ttu-id="1de5d-199">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-199">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="1de5d-200">Batch</span><span class="sxs-lookup"><span data-stu-id="1de5d-200">Batch</span></span>

* <span data-ttu-id="1de5d-201">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="1de5d-201">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1de5d-202">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="1de5d-202">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1de5d-203">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="1de5d-203">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1de5d-204">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="1de5d-204">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1de5d-205">Batchai</span><span class="sxs-lookup"><span data-stu-id="1de5d-205">Batchai</span></span>

* <span data-ttu-id="1de5d-206">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="1de5d-206">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1de5d-207">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1de5d-207">Keyvault</span></span>

* <span data-ttu-id="1de5d-208">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1de5d-208">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1de5d-209">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1de5d-209">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1de5d-210">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-210">Network</span></span>

* <span data-ttu-id="1de5d-211">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="1de5d-211">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1de5d-212">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="1de5d-212">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-213">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-213">Resource</span></span>

* <span data-ttu-id="1de5d-214">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="1de5d-214">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="1de5d-215">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1de5d-215">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1de5d-216">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="1de5d-216">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1de5d-217">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="1de5d-217">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-218">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-218">Sql</span></span>

* <span data-ttu-id="1de5d-219">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="1de5d-219">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1de5d-220">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="1de5d-220">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1de5d-221">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="1de5d-221">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-222">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-222">Storage</span></span>

* <span data-ttu-id="1de5d-223">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="1de5d-223">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-224">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-224">Vm</span></span>

* <span data-ttu-id="1de5d-225">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="1de5d-225">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1de5d-226">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-226">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="1de5d-227">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1de5d-227">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="1de5d-228">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-228">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="1de5d-229">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-229">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="1de5d-230">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-230">September 22, 2017</span></span>

<span data-ttu-id="1de5d-231">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="1de5d-231">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-232">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-232">Resource</span></span>

* <span data-ttu-id="1de5d-233">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="1de5d-233">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1de5d-234">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="1de5d-234">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1de5d-235">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-235">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="1de5d-236">[CHANGEMENT RÉCENT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="1de5d-236">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-237">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-237">Network</span></span>

* <span data-ttu-id="1de5d-238">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="1de5d-238">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1de5d-239">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="1de5d-239">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="1de5d-240">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="1de5d-240">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1de5d-241">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-241">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="1de5d-242">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-242">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1de5d-243">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-243">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="1de5d-244">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-244">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-245">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-245">Storage</span></span>

* <span data-ttu-id="1de5d-246">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1de5d-246">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1de5d-247">Événement</span><span class="sxs-lookup"><span data-stu-id="1de5d-247">Eventgrid</span></span>

* <span data-ttu-id="1de5d-248">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="1de5d-248">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-249">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-249">SQL</span></span>

* <span data-ttu-id="1de5d-250">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="1de5d-250">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1de5d-251">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="1de5d-251">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1de5d-252">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-252">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="1de5d-253">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1de5d-253">Keyvault</span></span>

* <span data-ttu-id="1de5d-254">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="1de5d-254">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-255">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-255">VM</span></span>

* <span data-ttu-id="1de5d-256">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-256">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="1de5d-257">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="1de5d-257">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1de5d-258">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-258">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="1de5d-259">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="1de5d-259">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="1de5d-260">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="1de5d-260">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="1de5d-261">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1de5d-261">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-262">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-262">ACS</span></span>

* <span data-ttu-id="1de5d-263">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="1de5d-263">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-264">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-264">Appservice</span></span>

* <span data-ttu-id="1de5d-265">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-265">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1de5d-266">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="1de5d-266">Backup</span></span>

* <span data-ttu-id="1de5d-267">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="1de5d-267">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1de5d-268">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-268">September 11, 2017</span></span>

<span data-ttu-id="1de5d-269">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1de5d-269">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1de5d-270">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-270">Core</span></span>

* <span data-ttu-id="1de5d-271">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="1de5d-271">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1de5d-272">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="1de5d-272">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-273">Acs</span><span class="sxs-lookup"><span data-stu-id="1de5d-273">Acs</span></span>

* <span data-ttu-id="1de5d-274">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="1de5d-274">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1de5d-275">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="1de5d-275">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-276">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-276">Appservice</span></span>

* <span data-ttu-id="1de5d-277">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="1de5d-277">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1de5d-278">CDN</span><span class="sxs-lookup"><span data-stu-id="1de5d-278">CDN</span></span>

* <span data-ttu-id="1de5d-279">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-279">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="1de5d-280">Extension</span><span class="sxs-lookup"><span data-stu-id="1de5d-280">Extension</span></span>

* <span data-ttu-id="1de5d-281">Version initiale.</span><span class="sxs-lookup"><span data-stu-id="1de5d-281">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="1de5d-282">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1de5d-282">Keyvault</span></span>

* <span data-ttu-id="1de5d-283">Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-283">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-284">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-284">Network</span></span>

* <span data-ttu-id="1de5d-285">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1de5d-285">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1de5d-286">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-286">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="1de5d-287">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-287">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="1de5d-288">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-288">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1de5d-289">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-289">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-290">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-290">Resource</span></span>

* <span data-ttu-id="1de5d-291">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-291">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="1de5d-292">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-292">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="1de5d-293">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="1de5d-293">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1de5d-294">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="1de5d-294">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-295">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-295">SQL</span></span>

* <span data-ttu-id="1de5d-296">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="1de5d-296">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-297">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-297">VM</span></span>

* <span data-ttu-id="1de5d-298">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="1de5d-298">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1de5d-299">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="1de5d-299">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1de5d-300">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-300">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1de5d-301">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="1de5d-301">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1de5d-302">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="1de5d-302">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1de5d-303">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-303">August 31, 2017</span></span>

<span data-ttu-id="1de5d-304">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1de5d-304">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1de5d-305">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1de5d-305">Keyvault</span></span>

* <span data-ttu-id="1de5d-306">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="1de5d-306">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="1de5d-307">Sf</span><span class="sxs-lookup"><span data-stu-id="1de5d-307">Sf</span></span>

* <span data-ttu-id="1de5d-308">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="1de5d-308">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-309">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-309">Storage</span></span>

* <span data-ttu-id="1de5d-310">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="1de5d-310">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1de5d-311">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="1de5d-311">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1de5d-312">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-312">August 28, 2017</span></span>

<span data-ttu-id="1de5d-313">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1de5d-313">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1de5d-314">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="1de5d-314">CLI</span></span>

* <span data-ttu-id="1de5d-315">Ajout d’une remarque juridique pour `--version`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-315">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-316">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-316">ACS</span></span>

* <span data-ttu-id="1de5d-317">Correction des régions d’aperçu.</span><span class="sxs-lookup"><span data-stu-id="1de5d-317">Corrected preview regions.</span></span>
* <span data-ttu-id="1de5d-318">Mise en forme par défaut `dns_name_prefix` correctement.</span><span class="sxs-lookup"><span data-stu-id="1de5d-318">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="1de5d-319">Sortie de commande des services ACS optimisée.</span><span class="sxs-lookup"><span data-stu-id="1de5d-319">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-320">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-320">Appservice</span></span>

* <span data-ttu-id="1de5d-321">[MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-321">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="1de5d-322">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="1de5d-322">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="1de5d-323">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="1de5d-323">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="1de5d-324">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="1de5d-324">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1de5d-325">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="1de5d-325">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1de5d-326">IoT</span><span class="sxs-lookup"><span data-stu-id="1de5d-326">IoT</span></span>

* <span data-ttu-id="1de5d-327">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="1de5d-327">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-328">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-328">Network</span></span>

* <span data-ttu-id="1de5d-329">[MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1de5d-329">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1de5d-330">[MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-330">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="1de5d-331">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1de5d-331">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1de5d-332">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-332">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1de5d-333">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-333">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="1de5d-334">Profil</span><span class="sxs-lookup"><span data-stu-id="1de5d-334">Profile</span></span>

* <span data-ttu-id="1de5d-335">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-335">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1de5d-336">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1de5d-336">Service Fabric</span></span>

* <span data-ttu-id="1de5d-337">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="1de5d-337">Preview release</span></span>
* <span data-ttu-id="1de5d-338">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="1de5d-338">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1de5d-339">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="1de5d-339">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1de5d-340">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="1de5d-340">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-341">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-341">Storage</span></span>

* <span data-ttu-id="1de5d-342">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="1de5d-342">Enabled setting blob tier</span></span>
* <span data-ttu-id="1de5d-343">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="1de5d-343">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1de5d-344">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="1de5d-344">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="1de5d-345">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="1de5d-345">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1de5d-346">[MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande</span><span class="sxs-lookup"><span data-stu-id="1de5d-346">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1de5d-347">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="1de5d-347">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-348">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-348">VM</span></span>

* <span data-ttu-id="1de5d-349">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="1de5d-349">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="1de5d-350">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="1de5d-350">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="1de5d-351">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-351">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="1de5d-352">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="1de5d-352">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1de5d-353">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="1de5d-353">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1de5d-354">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-354">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="1de5d-355">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-355">August 15, 2017</span></span>

<span data-ttu-id="1de5d-356">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1de5d-356">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-357">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-357">ACS</span></span>

* <span data-ttu-id="1de5d-358">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="1de5d-358">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-359">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-359">Appservice</span></span>

* <span data-ttu-id="1de5d-360">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="1de5d-360">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1de5d-361">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1de5d-361">Event Grid</span></span>

* <span data-ttu-id="1de5d-362">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1de5d-362">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1de5d-363">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-363">August 11, 2017</span></span>

<span data-ttu-id="1de5d-364">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1de5d-364">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-365">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-365">ACS</span></span>

* <span data-ttu-id="1de5d-366">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="1de5d-366">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1de5d-367">Batch</span><span class="sxs-lookup"><span data-stu-id="1de5d-367">Batch</span></span>

* <span data-ttu-id="1de5d-368">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1de5d-368">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1de5d-369">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="1de5d-369">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1de5d-370">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="1de5d-370">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1de5d-371">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="1de5d-371">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1de5d-372">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="1de5d-372">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1de5d-373">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="1de5d-373">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1de5d-374">Composant</span><span class="sxs-lookup"><span data-stu-id="1de5d-374">Component</span></span>

* <span data-ttu-id="1de5d-375">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="1de5d-375">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1de5d-376">Conteneur</span><span class="sxs-lookup"><span data-stu-id="1de5d-376">Container</span></span>

* <span data-ttu-id="1de5d-377">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="1de5d-377">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1de5d-378">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1de5d-378">Data Lake Store</span></span>

* <span data-ttu-id="1de5d-379">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="1de5d-379">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1de5d-380">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1de5d-380">Event Grid</span></span>

* <span data-ttu-id="1de5d-381">Version initiale</span><span class="sxs-lookup"><span data-stu-id="1de5d-381">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-382">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-382">Network</span></span>

* <span data-ttu-id="1de5d-383">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="1de5d-383">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="1de5d-384">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="1de5d-384">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="1de5d-385">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="1de5d-385">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1de5d-386">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="1de5d-386">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="1de5d-387">Profil</span><span class="sxs-lookup"><span data-stu-id="1de5d-387">Profile</span></span>

* <span data-ttu-id="1de5d-388">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="1de5d-388">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-389">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-389">Storage</span></span>

* <span data-ttu-id="1de5d-390">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="1de5d-390">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-391">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-391">VM</span></span>

* <span data-ttu-id="1de5d-392">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="1de5d-392">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1de5d-393">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="1de5d-393">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1de5d-394">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="1de5d-394">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1de5d-395">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="1de5d-395">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1de5d-396">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="1de5d-396">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1de5d-397">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-397">July 28, 2017</span></span>

<span data-ttu-id="1de5d-398">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1de5d-398">Version 2.0.12</span></span>

* <span data-ttu-id="1de5d-399">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="1de5d-399">Added container commands</span></span>
* <span data-ttu-id="1de5d-400">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="1de5d-400">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1de5d-401">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-401">Core</span></span>

* <span data-ttu-id="1de5d-402">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="1de5d-402">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1de5d-403">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="1de5d-403">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1de5d-404">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="1de5d-404">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1de5d-405">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="1de5d-405">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1de5d-406">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="1de5d-406">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1de5d-407">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="1de5d-407">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1de5d-408">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="1de5d-408">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1de5d-409">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="1de5d-409">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1de5d-410">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="1de5d-410">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1de5d-411">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1de5d-411">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1de5d-412">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="1de5d-412">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1de5d-413">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="1de5d-413">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1de5d-414">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="1de5d-414">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1de5d-415">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="1de5d-415">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1de5d-416">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1de5d-416">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1de5d-417">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="1de5d-417">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1de5d-418">ACR</span><span class="sxs-lookup"><span data-stu-id="1de5d-418">ACR</span></span>

* <span data-ttu-id="1de5d-419">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="1de5d-419">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1de5d-420">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="1de5d-420">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1de5d-421">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="1de5d-421">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1de5d-422">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="1de5d-422">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1de5d-423">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="1de5d-423">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1de5d-424">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="1de5d-424">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-425">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-425">ACS</span></span>

* <span data-ttu-id="1de5d-426">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="1de5d-426">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-427">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-427">Appservice</span></span>

* <span data-ttu-id="1de5d-428">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="1de5d-428">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1de5d-429">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="1de5d-429">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1de5d-430">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="1de5d-430">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="1de5d-431">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="1de5d-431">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1de5d-432">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="1de5d-432">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1de5d-433">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="1de5d-433">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1de5d-434">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="1de5d-434">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1de5d-435">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="1de5d-435">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1de5d-436">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="1de5d-436">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1de5d-437">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="1de5d-437">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="1de5d-438">Batch</span><span class="sxs-lookup"><span data-stu-id="1de5d-438">Batch</span></span>

* <span data-ttu-id="1de5d-439">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="1de5d-439">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1de5d-440">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="1de5d-440">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="1de5d-441">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="1de5d-441">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="1de5d-442">CDN</span><span class="sxs-lookup"><span data-stu-id="1de5d-442">CDN</span></span>

* <span data-ttu-id="1de5d-443">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="1de5d-443">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="1de5d-444">Cloud</span><span class="sxs-lookup"><span data-stu-id="1de5d-444">Cloud</span></span>

* <span data-ttu-id="1de5d-445">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="1de5d-445">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1de5d-446">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="1de5d-446">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1de5d-447">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="1de5d-447">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1de5d-448">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="1de5d-448">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1de5d-449">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="1de5d-449">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1de5d-450">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1de5d-450">CosmosDB</span></span>

* <span data-ttu-id="1de5d-451">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="1de5d-451">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1de5d-452">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="1de5d-452">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1de5d-453">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1de5d-453">Data Lake Analytics</span></span>

* <span data-ttu-id="1de5d-454">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="1de5d-454">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1de5d-455">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="1de5d-455">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="1de5d-456">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="1de5d-456">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1de5d-457">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1de5d-457">Data Lake Store</span></span>

* <span data-ttu-id="1de5d-458">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-458">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="1de5d-459">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="1de5d-459">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1de5d-460">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-460">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1de5d-461">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1de5d-461">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1de5d-462">Interactive</span><span class="sxs-lookup"><span data-stu-id="1de5d-462">Interactive</span></span>

* <span data-ttu-id="1de5d-463">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="1de5d-463">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1de5d-464">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="1de5d-464">Increased test coverage</span></span>
* <span data-ttu-id="1de5d-465">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="1de5d-465">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1de5d-466">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="1de5d-466">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1de5d-467">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="1de5d-467">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1de5d-468">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="1de5d-468">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1de5d-469">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="1de5d-469">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1de5d-470">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="1de5d-470">Added `--progress` flag</span></span>
* <span data-ttu-id="1de5d-471">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="1de5d-471">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1de5d-472">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="1de5d-472">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1de5d-473">IoT</span><span class="sxs-lookup"><span data-stu-id="1de5d-473">IoT</span></span>

* <span data-ttu-id="1de5d-474">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="1de5d-474">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1de5d-475">(#3934)</span><span class="sxs-lookup"><span data-stu-id="1de5d-475">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1de5d-476">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="1de5d-476">Key vault</span></span>

* <span data-ttu-id="1de5d-477">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="1de5d-477">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="1de5d-478">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1de5d-478">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="1de5d-479">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1de5d-479">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1de5d-480">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1de5d-480">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1de5d-481">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="1de5d-481">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="1de5d-482">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="1de5d-482">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1de5d-483">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="1de5d-483">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1de5d-484">(#3307)</span><span class="sxs-lookup"><span data-stu-id="1de5d-484">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1de5d-485">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1de5d-485">Lab</span></span>

* <span data-ttu-id="1de5d-486">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="1de5d-486">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="1de5d-487">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="1de5d-487">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="1de5d-488">Surveiller</span><span class="sxs-lookup"><span data-stu-id="1de5d-488">Monitor</span></span>

* <span data-ttu-id="1de5d-489">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="1de5d-489">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1de5d-490">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="1de5d-490">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="1de5d-491">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="1de5d-491">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="1de5d-492">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="1de5d-492">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="1de5d-493">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="1de5d-493">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="1de5d-494">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="1de5d-494">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="1de5d-495">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="1de5d-495">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1de5d-496">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="1de5d-496">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="1de5d-497">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="1de5d-497">`location` no longer required</span></span>
  * <span data-ttu-id="1de5d-498">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="1de5d-498">Add name and ID support for target</span></span>
  * <span data-ttu-id="1de5d-499">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="1de5d-499">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="1de5d-500">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="1de5d-500">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="1de5d-501">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="1de5d-501">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1de5d-502">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="1de5d-502">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1de5d-503">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="1de5d-503">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1de5d-504">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-504">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-505">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-505">Network</span></span>

* <span data-ttu-id="1de5d-506">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="1de5d-506">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1de5d-507">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-507">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="1de5d-508">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="1de5d-508">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1de5d-509">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="1de5d-509">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1de5d-510">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-510">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="1de5d-511">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1de5d-511">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1de5d-512">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="1de5d-512">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="1de5d-513">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="1de5d-513">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="1de5d-514">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="1de5d-514">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1de5d-515">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1de5d-515">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="1de5d-516">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-516">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="1de5d-517">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="1de5d-517">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="1de5d-518">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="1de5d-518">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="1de5d-519">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-519">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="1de5d-520">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-520">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="1de5d-521">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-521">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="1de5d-522">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="1de5d-522">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1de5d-523">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1de5d-523">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="1de5d-524">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-524">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="1de5d-525">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-525">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="1de5d-526">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-526">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="1de5d-527">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="1de5d-527">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1de5d-528">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="1de5d-528">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="1de5d-529">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1de5d-529">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1de5d-530">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1de5d-530">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1de5d-531">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1de5d-531">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1de5d-532">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="1de5d-532">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1de5d-533">Profil</span><span class="sxs-lookup"><span data-stu-id="1de5d-533">Profile</span></span>

* <span data-ttu-id="1de5d-534">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="1de5d-534">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1de5d-535">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="1de5d-535">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1de5d-536">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="1de5d-536">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1de5d-537">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="1de5d-537">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1de5d-538">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="1de5d-538">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1de5d-539">SGBDR</span><span class="sxs-lookup"><span data-stu-id="1de5d-539">RDBMS</span></span>

* <span data-ttu-id="1de5d-540">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="1de5d-540">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1de5d-541">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="1de5d-541">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1de5d-542">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="1de5d-542">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1de5d-543">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="1de5d-543">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-544">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-544">Resource</span></span>

* <span data-ttu-id="1de5d-545">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-545">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="1de5d-546">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1de5d-546">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1de5d-547">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1de5d-547">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1de5d-548">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="1de5d-548">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1de5d-549">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="1de5d-549">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1de5d-550">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="1de5d-550">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="1de5d-551">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="1de5d-551">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1de5d-552">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="1de5d-552">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1de5d-553">Rôle</span><span class="sxs-lookup"><span data-stu-id="1de5d-553">Role</span></span>

* <span data-ttu-id="1de5d-554">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1de5d-554">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="1de5d-555">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="1de5d-555">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1de5d-556">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="1de5d-556">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1de5d-557">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="1de5d-557">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="1de5d-558">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="1de5d-558">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1de5d-559">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1de5d-559">Service Fabric</span></span>
* <span data-ttu-id="1de5d-560">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="1de5d-560">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1de5d-561">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="1de5d-561">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1de5d-562">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="1de5d-562">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-563">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-563">SQL</span></span>

* <span data-ttu-id="1de5d-564">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="1de5d-564">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1de5d-565">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="1de5d-565">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1de5d-566">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="1de5d-566">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-567">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-567">Storage</span></span>

* <span data-ttu-id="1de5d-568">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="1de5d-568">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1de5d-569">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="1de5d-569">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1de5d-570">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="1de5d-570">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1de5d-571">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="1de5d-571">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="1de5d-572">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="1de5d-572">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="1de5d-573">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="1de5d-573">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-574">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-574">VM</span></span>

* <span data-ttu-id="1de5d-575">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-575">Support configuring nsg</span></span>
* <span data-ttu-id="1de5d-576">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="1de5d-576">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1de5d-577">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="1de5d-577">Support managed service identities</span></span>
* <span data-ttu-id="1de5d-578">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-578">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="1de5d-579">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="1de5d-579">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1de5d-580">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-580">May 10, 2017</span></span>

<span data-ttu-id="1de5d-581">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1de5d-581">Version 2.0.6</span></span>

* <span data-ttu-id="1de5d-582">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1de5d-582">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1de5d-583">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="1de5d-583">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1de5d-584">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1de5d-584">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="1de5d-585">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="1de5d-585">Include Cognitive Services module.</span></span>
* <span data-ttu-id="1de5d-586">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="1de5d-586">Include Service Fabric module.</span></span>
* <span data-ttu-id="1de5d-587">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="1de5d-587">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="1de5d-588">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="1de5d-588">Add support for CDN commands.</span></span>
* <span data-ttu-id="1de5d-589">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="1de5d-589">Remove Container module.</span></span>
* <span data-ttu-id="1de5d-590">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="1de5d-590">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1de5d-591">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1de5d-591">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1de5d-592">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-592">Core</span></span>

* <span data-ttu-id="1de5d-593">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="1de5d-593">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="1de5d-594">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="1de5d-594">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1de5d-595">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="1de5d-595">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1de5d-596">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="1de5d-596">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1de5d-597">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="1de5d-597">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1de5d-598">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="1de5d-598">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1de5d-599">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="1de5d-599">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1de5d-600">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="1de5d-600">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1de5d-601">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="1de5d-601">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1de5d-602">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="1de5d-602">core: Improved performance</span></span>
* <span data-ttu-id="1de5d-603">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="1de5d-603">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1de5d-604">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="1de5d-604">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1de5d-605">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-605">ACS</span></span>

* <span data-ttu-id="1de5d-606">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="1de5d-606">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1de5d-607">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="1de5d-607">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1de5d-608">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="1de5d-608">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1de5d-609">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="1de5d-609">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1de5d-610">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-610">AppService</span></span>

* <span data-ttu-id="1de5d-611">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="1de5d-611">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1de5d-612">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="1de5d-612">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1de5d-613">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="1de5d-613">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1de5d-614">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="1de5d-614">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1de5d-615">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="1de5d-615">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1de5d-616">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="1de5d-616">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1de5d-617">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="1de5d-617">support slot swap with preview</span></span>
* <span data-ttu-id="1de5d-618">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="1de5d-618">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1de5d-619">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="1de5d-619">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1de5d-620">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1de5d-620">CosmosDB</span></span>

* <span data-ttu-id="1de5d-621">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="1de5d-621">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="1de5d-622">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="1de5d-622">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1de5d-623">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="1de5d-623">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1de5d-624">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="1de5d-624">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1de5d-625">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1de5d-625">Data Lake Analytics</span></span>

* <span data-ttu-id="1de5d-626">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="1de5d-626">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="1de5d-627">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="1de5d-627">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1de5d-628">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="1de5d-628">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="1de5d-629">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="1de5d-629">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1de5d-630">Table</span><span class="sxs-lookup"><span data-stu-id="1de5d-630">Table</span></span>
  * <span data-ttu-id="1de5d-631">Fonction table</span><span class="sxs-lookup"><span data-stu-id="1de5d-631">Table valued function</span></span>
  * <span data-ttu-id="1de5d-632">Affichage</span><span class="sxs-lookup"><span data-stu-id="1de5d-632">View</span></span>
  * <span data-ttu-id="1de5d-633">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="1de5d-633">Table Statistics.</span></span> <span data-ttu-id="1de5d-634">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="1de5d-634">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1de5d-635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1de5d-635">Data Lake Store</span></span>

* <span data-ttu-id="1de5d-636">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="1de5d-636">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="1de5d-637">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1de5d-637">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1de5d-638">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="1de5d-638">missed help for access show.</span></span> <span data-ttu-id="1de5d-639">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="1de5d-639">adding it.</span></span> <span data-ttu-id="1de5d-640">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1de5d-640">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1de5d-641">Rechercher</span><span class="sxs-lookup"><span data-stu-id="1de5d-641">Find</span></span>

* <span data-ttu-id="1de5d-642">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="1de5d-642">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1de5d-643">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1de5d-643">KeyVault</span></span>

* <span data-ttu-id="1de5d-644">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="1de5d-644">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1de5d-645">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="1de5d-645">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="1de5d-646">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="1de5d-646">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1de5d-647">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="1de5d-647">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="1de5d-648">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="1de5d-648">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1de5d-649">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="1de5d-649">Lab</span></span>

* <span data-ttu-id="1de5d-650">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="1de5d-650">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="1de5d-651">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="1de5d-651">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="1de5d-652">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="1de5d-652">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="1de5d-653">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="1de5d-653">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="1de5d-654">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="1de5d-654">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="1de5d-655">Surveiller</span><span class="sxs-lookup"><span data-stu-id="1de5d-655">Monitor</span></span>

* <span data-ttu-id="1de5d-656">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="1de5d-656">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1de5d-657">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="1de5d-657">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1de5d-658">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-658">Network</span></span>

* <span data-ttu-id="1de5d-659">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-659">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="1de5d-660">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-660">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="1de5d-661">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="1de5d-661">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="1de5d-662">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="1de5d-662">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="1de5d-663">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1de5d-663">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="1de5d-664">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="1de5d-664">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="1de5d-665">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="1de5d-665">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="1de5d-666">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="1de5d-666">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="1de5d-667">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-667">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="1de5d-668">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="1de5d-668">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1de5d-669">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-669">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="1de5d-670">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1de5d-670">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="1de5d-671">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="1de5d-671">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="1de5d-672">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="1de5d-672">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="1de5d-673">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="1de5d-673">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="1de5d-674">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="1de5d-674">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="1de5d-675">Profil</span><span class="sxs-lookup"><span data-stu-id="1de5d-675">Profile</span></span>

* <span data-ttu-id="1de5d-676">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="1de5d-676">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1de5d-677">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="1de5d-677">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1de5d-678">Redis</span><span class="sxs-lookup"><span data-stu-id="1de5d-678">Redis</span></span>

* <span data-ttu-id="1de5d-679">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="1de5d-679">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1de5d-680">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="1de5d-680">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="1de5d-681">Ressource</span><span class="sxs-lookup"><span data-stu-id="1de5d-681">Resource</span></span>

* <span data-ttu-id="1de5d-682">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="1de5d-682">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1de5d-683">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="1de5d-683">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1de5d-684">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="1de5d-684">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1de5d-685">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="1de5d-685">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1de5d-686">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1de5d-686">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1de5d-687">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="1de5d-687">Add docs for az lock update.</span></span> <span data-ttu-id="1de5d-688">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1de5d-688">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1de5d-689">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="1de5d-689">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1de5d-690">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1de5d-690">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1de5d-691">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="1de5d-691">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1de5d-692">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1de5d-692">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1de5d-693">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="1de5d-693">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1de5d-694">Rôle</span><span class="sxs-lookup"><span data-stu-id="1de5d-694">Role</span></span>

* <span data-ttu-id="1de5d-695">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="1de5d-695">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1de5d-696">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="1de5d-696">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1de5d-697">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="1de5d-697">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1de5d-698">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="1de5d-698">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1de5d-699">SQL</span><span class="sxs-lookup"><span data-stu-id="1de5d-699">SQL</span></span>

* <span data-ttu-id="1de5d-700">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="1de5d-700">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="1de5d-701">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="1de5d-701">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1de5d-702">Storage</span><span class="sxs-lookup"><span data-stu-id="1de5d-702">Storage</span></span>

* <span data-ttu-id="1de5d-703">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-703">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="1de5d-704">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="1de5d-704">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1de5d-705">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="1de5d-705">Add support for large block blob upload</span></span>
* <span data-ttu-id="1de5d-706">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="1de5d-706">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-707">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-707">VM</span></span>

* <span data-ttu-id="1de5d-708">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="1de5d-708">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1de5d-709">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="1de5d-709">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1de5d-710">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1de5d-710">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1de5d-711">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1de5d-711">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1de5d-712">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="1de5d-712">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1de5d-713">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="1de5d-713">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1de5d-714">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="1de5d-714">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1de5d-715">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-715">April 3, 2017</span></span>

<span data-ttu-id="1de5d-716">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1de5d-716">Version 2.0.2</span></span>

<span data-ttu-id="1de5d-717">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="1de5d-717">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="1de5d-718">Principal</span><span class="sxs-lookup"><span data-stu-id="1de5d-718">Core</span></span>

* <span data-ttu-id="1de5d-719">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="1de5d-719">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="1de5d-720">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="1de5d-720">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1de5d-721">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="1de5d-721">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1de5d-722">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1de5d-722">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1de5d-723">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="1de5d-723">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1de5d-724">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="1de5d-724">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1de5d-725">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="1de5d-725">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1de5d-726">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="1de5d-726">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1de5d-727">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="1de5d-727">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="1de5d-728">ACS</span><span class="sxs-lookup"><span data-stu-id="1de5d-728">ACS</span></span>

* <span data-ttu-id="1de5d-729">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="1de5d-729">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1de5d-730">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="1de5d-730">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1de5d-731">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="1de5d-731">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1de5d-732">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="1de5d-732">Add support for windows clusters.</span></span> <span data-ttu-id="1de5d-733">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="1de5d-733">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1de5d-734">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="1de5d-734">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1de5d-735">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="1de5d-735">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="1de5d-736">AppService</span><span class="sxs-lookup"><span data-stu-id="1de5d-736">AppService</span></span>

* <span data-ttu-id="1de5d-737">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="1de5d-737">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1de5d-738">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="1de5d-738">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1de5d-739">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="1de5d-739">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1de5d-740">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="1de5d-740">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="1de5d-741">DataLake</span><span class="sxs-lookup"><span data-stu-id="1de5d-741">DataLake</span></span>

* <span data-ttu-id="1de5d-742">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="1de5d-742">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="1de5d-743">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1de5d-743">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="1de5d-744">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="1de5d-744">DocuemntDB</span></span>

* <span data-ttu-id="1de5d-745">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="1de5d-745">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1de5d-746">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="1de5d-746">VM</span></span>

* <span data-ttu-id="1de5d-747">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="1de5d-747">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1de5d-748">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="1de5d-748">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1de5d-749">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="1de5d-749">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1de5d-750">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1de5d-750">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1de5d-751">Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="1de5d-751">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1de5d-752">Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="1de5d-752">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="1de5d-753">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="1de5d-753">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1de5d-754">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="1de5d-754">February 27, 2017</span></span>

<span data-ttu-id="1de5d-755">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1de5d-755">Version 2.0.0</span></span>

<span data-ttu-id="1de5d-756">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="1de5d-756">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="1de5d-757">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="1de5d-757">General availability applies to these command modules:</span></span>
- <span data-ttu-id="1de5d-758">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="1de5d-758">Container Service (acs)</span></span>
- <span data-ttu-id="1de5d-759">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="1de5d-759">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1de5d-760">Réseau</span><span class="sxs-lookup"><span data-stu-id="1de5d-760">Networking</span></span>
- <span data-ttu-id="1de5d-761">Stockage</span><span class="sxs-lookup"><span data-stu-id="1de5d-761">Storage</span></span>

<span data-ttu-id="1de5d-762">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="1de5d-762">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="1de5d-763">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="1de5d-763">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="1de5d-764">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-764">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="1de5d-765">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1de5d-765">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="1de5d-766">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-766">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="1de5d-767">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="1de5d-767">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="1de5d-768">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="1de5d-768">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="1de5d-769">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="1de5d-769">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="1de5d-770">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="1de5d-770">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="1de5d-771">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="1de5d-771">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="1de5d-772">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="1de5d-772">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1de5d-773">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="1de5d-773">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1de5d-774">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1de5d-774">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="1de5d-775">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1de5d-775">Provide feedback from the command line with the `az feedback` command.</span></span>

