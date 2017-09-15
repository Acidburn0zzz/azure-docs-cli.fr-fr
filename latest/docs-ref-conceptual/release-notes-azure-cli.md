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
ms.openlocfilehash: ad30efeb7efafcc5816160ee130665d37adb62c6
ms.sourcegitcommit: e866977985ba0286fa05f41729dd7e7d9ce86f8e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/13/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="77103-104">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="77103-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-11-2017"></a><span data-ttu-id="77103-105">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="77103-105">September 11, 2017</span></span>

<span data-ttu-id="77103-106">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="77103-106">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="77103-107">Principal</span><span class="sxs-lookup"><span data-stu-id="77103-107">Core</span></span>

* <span data-ttu-id="77103-108">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="77103-108">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="77103-109">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="77103-109">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="77103-110">Acs</span><span class="sxs-lookup"><span data-stu-id="77103-110">Acs</span></span>

* <span data-ttu-id="77103-111">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="77103-111">Added `acs list-locations` command</span></span>
* <span data-ttu-id="77103-112">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="77103-112">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="77103-113">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-113">Appservice</span></span>

* <span data-ttu-id="77103-114">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="77103-114">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="77103-115">CDN</span><span class="sxs-lookup"><span data-stu-id="77103-115">CDN</span></span>

* <span data-ttu-id="77103-116">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="77103-116">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="77103-117">Extension</span><span class="sxs-lookup"><span data-stu-id="77103-117">Extension</span></span>

* <span data-ttu-id="77103-118">Version initiale.</span><span class="sxs-lookup"><span data-stu-id="77103-118">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="77103-119">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77103-119">Keyvault</span></span>

* <span data-ttu-id="77103-120">Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="77103-120">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="77103-121">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-121">Network</span></span>

* <span data-ttu-id="77103-122">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="77103-122">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="77103-123">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="77103-123">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="77103-124">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="77103-124">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="77103-125">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="77103-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="77103-126">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="77103-126">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="77103-127">Ressource</span><span class="sxs-lookup"><span data-stu-id="77103-127">Resource</span></span>

* <span data-ttu-id="77103-128">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="77103-128">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="77103-129">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="77103-129">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="77103-130">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="77103-130">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="77103-131">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="77103-131">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="77103-132">SQL</span><span class="sxs-lookup"><span data-stu-id="77103-132">SQL</span></span>

* <span data-ttu-id="77103-133">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="77103-133">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="77103-134">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-134">VM</span></span>

* <span data-ttu-id="77103-135">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="77103-135">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="77103-136">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="77103-136">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="77103-137">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77103-137">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="77103-138">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="77103-138">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="77103-139">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="77103-139">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="77103-140">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="77103-140">August 31, 2017</span></span>

<span data-ttu-id="77103-141">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="77103-141">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="77103-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77103-142">Keyvault</span></span>

* <span data-ttu-id="77103-143">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="77103-143">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="77103-144">Sf</span><span class="sxs-lookup"><span data-stu-id="77103-144">Sf</span></span>

* <span data-ttu-id="77103-145">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="77103-145">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="77103-146">Storage</span><span class="sxs-lookup"><span data-stu-id="77103-146">Storage</span></span>

* <span data-ttu-id="77103-147">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="77103-147">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="77103-148">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="77103-148">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="77103-149">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="77103-149">August 28, 2017</span></span>

<span data-ttu-id="77103-150">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="77103-150">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="77103-151">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="77103-151">CLI</span></span>

* <span data-ttu-id="77103-152">Ajout d’une remarque juridique pour `--version`.</span><span class="sxs-lookup"><span data-stu-id="77103-152">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="77103-153">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-153">ACS</span></span>

* <span data-ttu-id="77103-154">Correction des régions d’aperçu.</span><span class="sxs-lookup"><span data-stu-id="77103-154">Corrected preview regions.</span></span>
* <span data-ttu-id="77103-155">Mise en forme par défaut `dns_name_prefix` correctement.</span><span class="sxs-lookup"><span data-stu-id="77103-155">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="77103-156">Sortie de commande des services ACS optimisée.</span><span class="sxs-lookup"><span data-stu-id="77103-156">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="77103-157">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-157">Appservice</span></span>

* <span data-ttu-id="77103-158">[MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="77103-158">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="77103-159">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="77103-159">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="77103-160">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="77103-160">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="77103-161">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="77103-161">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="77103-162">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="77103-162">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="77103-163">IoT</span><span class="sxs-lookup"><span data-stu-id="77103-163">IoT</span></span>

* <span data-ttu-id="77103-164">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="77103-164">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="77103-165">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-165">Network</span></span>

* <span data-ttu-id="77103-166">[MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="77103-166">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="77103-167">[MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77103-167">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="77103-168">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="77103-168">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="77103-169">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="77103-169">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="77103-170">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="77103-170">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="77103-171">Profil</span><span class="sxs-lookup"><span data-stu-id="77103-171">Profile</span></span>

* <span data-ttu-id="77103-172">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-172">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77103-173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77103-173">Service Fabric</span></span>

* <span data-ttu-id="77103-174">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="77103-174">Preview release</span></span>
* <span data-ttu-id="77103-175">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="77103-175">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="77103-176">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="77103-176">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="77103-177">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="77103-177">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="77103-178">Storage</span><span class="sxs-lookup"><span data-stu-id="77103-178">Storage</span></span>

* <span data-ttu-id="77103-179">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="77103-179">Enabled setting blob tier</span></span>
* <span data-ttu-id="77103-180">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="77103-180">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="77103-181">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="77103-181">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="77103-182">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="77103-182">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="77103-183">[MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande</span><span class="sxs-lookup"><span data-stu-id="77103-183">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="77103-184">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="77103-184">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="77103-185">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-185">VM</span></span>

* <span data-ttu-id="77103-186">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="77103-186">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="77103-187">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="77103-187">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="77103-188">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="77103-188">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="77103-189">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="77103-189">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="77103-190">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="77103-190">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="77103-191">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="77103-191">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="77103-192">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="77103-192">August 15, 2017</span></span>

<span data-ttu-id="77103-193">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="77103-193">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="77103-194">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-194">ACS</span></span>

* <span data-ttu-id="77103-195">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="77103-195">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="77103-196">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-196">Appservice</span></span>

* <span data-ttu-id="77103-197">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="77103-197">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="77103-198">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77103-198">Event Grid</span></span>

* <span data-ttu-id="77103-199">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77103-199">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="77103-200">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="77103-200">August 11, 2017</span></span>

<span data-ttu-id="77103-201">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="77103-201">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="77103-202">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-202">ACS</span></span>

* <span data-ttu-id="77103-203">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="77103-203">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="77103-204">Batch</span><span class="sxs-lookup"><span data-stu-id="77103-204">Batch</span></span>

* <span data-ttu-id="77103-205">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="77103-205">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="77103-206">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="77103-206">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="77103-207">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="77103-207">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="77103-208">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="77103-208">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="77103-209">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="77103-209">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="77103-210">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="77103-210">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="77103-211">Composant</span><span class="sxs-lookup"><span data-stu-id="77103-211">Component</span></span>

* <span data-ttu-id="77103-212">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="77103-212">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="77103-213">Conteneur</span><span class="sxs-lookup"><span data-stu-id="77103-213">Container</span></span>

* <span data-ttu-id="77103-214">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="77103-214">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="77103-215">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77103-215">Data Lake Store</span></span>

* <span data-ttu-id="77103-216">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="77103-216">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="77103-217">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77103-217">Event Grid</span></span>

* <span data-ttu-id="77103-218">Version initiale</span><span class="sxs-lookup"><span data-stu-id="77103-218">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="77103-219">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-219">Network</span></span>

* <span data-ttu-id="77103-220">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="77103-220">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="77103-221">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="77103-221">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="77103-222">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="77103-222">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="77103-223">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="77103-223">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="77103-224">Profil</span><span class="sxs-lookup"><span data-stu-id="77103-224">Profile</span></span>

* <span data-ttu-id="77103-225">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="77103-225">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="77103-226">Storage</span><span class="sxs-lookup"><span data-stu-id="77103-226">Storage</span></span>

* <span data-ttu-id="77103-227">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="77103-227">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="77103-228">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-228">VM</span></span>

* <span data-ttu-id="77103-229">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="77103-229">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="77103-230">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="77103-230">Exposed `list-skus` command</span></span>
* <span data-ttu-id="77103-231">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="77103-231">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="77103-232">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="77103-232">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="77103-233">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="77103-233">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="77103-234">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="77103-234">July 28, 2017</span></span>

<span data-ttu-id="77103-235">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="77103-235">Version 2.0.12</span></span>

* <span data-ttu-id="77103-236">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="77103-236">Added container commands</span></span>
* <span data-ttu-id="77103-237">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="77103-237">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="77103-238">Principal</span><span class="sxs-lookup"><span data-stu-id="77103-238">Core</span></span>

* <span data-ttu-id="77103-239">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="77103-239">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="77103-240">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="77103-240">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="77103-241">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="77103-241">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="77103-242">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="77103-242">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="77103-243">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="77103-243">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="77103-244">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="77103-244">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="77103-245">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="77103-245">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77103-246">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="77103-246">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="77103-247">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="77103-247">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="77103-248">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77103-248">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="77103-249">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="77103-249">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="77103-250">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="77103-250">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="77103-251">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="77103-251">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="77103-252">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="77103-252">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="77103-253">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="77103-253">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="77103-254">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="77103-254">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="77103-255">ACR</span><span class="sxs-lookup"><span data-stu-id="77103-255">ACR</span></span>

* <span data-ttu-id="77103-256">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="77103-256">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="77103-257">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="77103-257">Support SKU update for managed registries</span></span>
* <span data-ttu-id="77103-258">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="77103-258">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="77103-259">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="77103-259">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="77103-260">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="77103-260">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="77103-261">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="77103-261">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="77103-262">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-262">ACS</span></span>

* <span data-ttu-id="77103-263">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="77103-263">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="77103-264">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-264">Appservice</span></span>

* <span data-ttu-id="77103-265">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="77103-265">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="77103-266">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="77103-266">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="77103-267">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="77103-267">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="77103-268">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="77103-268">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="77103-269">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="77103-269">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="77103-270">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="77103-270">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="77103-271">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="77103-271">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="77103-272">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="77103-272">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="77103-273">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="77103-273">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="77103-274">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="77103-274">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="77103-275">Batch</span><span class="sxs-lookup"><span data-stu-id="77103-275">Batch</span></span>

* <span data-ttu-id="77103-276">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="77103-276">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="77103-277">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="77103-277">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="77103-278">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="77103-278">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="77103-279">CDN</span><span class="sxs-lookup"><span data-stu-id="77103-279">CDN</span></span>

* <span data-ttu-id="77103-280">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="77103-280">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="77103-281">Cloud</span><span class="sxs-lookup"><span data-stu-id="77103-281">Cloud</span></span>

* <span data-ttu-id="77103-282">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="77103-282">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="77103-283">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="77103-283">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="77103-284">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="77103-284">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="77103-285">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="77103-285">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="77103-286">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="77103-286">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77103-287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77103-287">CosmosDB</span></span>

* <span data-ttu-id="77103-288">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="77103-288">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="77103-289">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="77103-289">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77103-290">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77103-290">Data Lake Analytics</span></span>

* <span data-ttu-id="77103-291">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="77103-291">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="77103-292">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="77103-292">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="77103-293">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="77103-293">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77103-294">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77103-294">Data Lake Store</span></span>

* <span data-ttu-id="77103-295">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="77103-295">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="77103-296">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="77103-296">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="77103-297">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="77103-297">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="77103-298">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77103-298">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="77103-299">Interactive</span><span class="sxs-lookup"><span data-stu-id="77103-299">Interactive</span></span>

* <span data-ttu-id="77103-300">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="77103-300">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="77103-301">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="77103-301">Increased test coverage</span></span>
* <span data-ttu-id="77103-302">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="77103-302">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="77103-303">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="77103-303">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="77103-304">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="77103-304">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="77103-305">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="77103-305">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="77103-306">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="77103-306">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77103-307">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="77103-307">Added `--progress` flag</span></span>
* <span data-ttu-id="77103-308">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="77103-308">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="77103-309">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="77103-309">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="77103-310">IoT</span><span class="sxs-lookup"><span data-stu-id="77103-310">IoT</span></span>

* <span data-ttu-id="77103-311">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="77103-311">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="77103-312">(#3934)</span><span class="sxs-lookup"><span data-stu-id="77103-312">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="77103-313">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="77103-313">Key vault</span></span>

* <span data-ttu-id="77103-314">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="77103-314">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="77103-315">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77103-315">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="77103-316">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77103-316">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77103-317">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77103-317">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77103-318">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77103-318">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="77103-319">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="77103-319">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="77103-320">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="77103-320">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="77103-321">(#3307)</span><span class="sxs-lookup"><span data-stu-id="77103-321">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="77103-322">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77103-322">Lab</span></span>

* <span data-ttu-id="77103-323">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="77103-323">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="77103-324">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="77103-324">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="77103-325">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77103-325">Monitor</span></span>

* <span data-ttu-id="77103-326">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="77103-326">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="77103-327">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="77103-327">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="77103-328">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="77103-328">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="77103-329">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="77103-329">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="77103-330">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="77103-330">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="77103-331">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="77103-331">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="77103-332">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="77103-332">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="77103-333">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="77103-333">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="77103-334">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="77103-334">`location` no longer required</span></span>
  * <span data-ttu-id="77103-335">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="77103-335">Add name and ID support for target</span></span>
  * <span data-ttu-id="77103-336">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="77103-336">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="77103-337">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="77103-337">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="77103-338">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="77103-338">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="77103-339">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="77103-339">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="77103-340">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="77103-340">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="77103-341">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="77103-341">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="77103-342">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-342">Network</span></span>

* <span data-ttu-id="77103-343">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="77103-343">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="77103-344">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="77103-344">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="77103-345">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="77103-345">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="77103-346">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="77103-346">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="77103-347">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="77103-347">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="77103-348">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="77103-348">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="77103-349">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="77103-349">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="77103-350">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="77103-350">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="77103-351">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="77103-351">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="77103-352">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="77103-352">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="77103-353">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="77103-353">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="77103-354">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="77103-354">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="77103-355">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="77103-355">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="77103-356">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="77103-356">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="77103-357">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="77103-357">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="77103-358">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="77103-358">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="77103-359">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="77103-359">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="77103-360">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="77103-360">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="77103-361">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="77103-361">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="77103-362">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="77103-362">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="77103-363">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="77103-363">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="77103-364">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="77103-364">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="77103-365">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="77103-365">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="77103-366">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77103-366">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="77103-367">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77103-367">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="77103-368">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77103-368">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="77103-369">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="77103-369">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="77103-370">Profil</span><span class="sxs-lookup"><span data-stu-id="77103-370">Profile</span></span>

* <span data-ttu-id="77103-371">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="77103-371">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="77103-372">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="77103-372">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="77103-373">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="77103-373">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="77103-374">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="77103-374">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="77103-375">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="77103-375">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="77103-376">SGBDR</span><span class="sxs-lookup"><span data-stu-id="77103-376">RDBMS</span></span>

* <span data-ttu-id="77103-377">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="77103-377">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="77103-378">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="77103-378">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="77103-379">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="77103-379">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="77103-380">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="77103-380">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="77103-381">Ressource</span><span class="sxs-lookup"><span data-stu-id="77103-381">Resource</span></span>

* <span data-ttu-id="77103-382">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="77103-382">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="77103-383">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77103-383">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="77103-384">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77103-384">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="77103-385">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="77103-385">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="77103-386">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="77103-386">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="77103-387">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="77103-387">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="77103-388">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="77103-388">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="77103-389">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="77103-389">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="77103-390">Rôle</span><span class="sxs-lookup"><span data-stu-id="77103-390">Role</span></span>

* <span data-ttu-id="77103-391">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="77103-391">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="77103-392">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="77103-392">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="77103-393">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="77103-393">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="77103-394">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="77103-394">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="77103-395">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="77103-395">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77103-396">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77103-396">Service Fabric</span></span>
* <span data-ttu-id="77103-397">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="77103-397">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="77103-398">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="77103-398">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="77103-399">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="77103-399">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="77103-400">SQL</span><span class="sxs-lookup"><span data-stu-id="77103-400">SQL</span></span>

* <span data-ttu-id="77103-401">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="77103-401">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="77103-402">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="77103-402">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="77103-403">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="77103-403">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="77103-404">Storage</span><span class="sxs-lookup"><span data-stu-id="77103-404">Storage</span></span>

* <span data-ttu-id="77103-405">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="77103-405">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="77103-406">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="77103-406">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="77103-407">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="77103-407">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="77103-408">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="77103-408">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="77103-409">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="77103-409">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="77103-410">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="77103-410">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="77103-411">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-411">VM</span></span>

* <span data-ttu-id="77103-412">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="77103-412">Support configuring nsg</span></span>
* <span data-ttu-id="77103-413">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="77103-413">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="77103-414">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="77103-414">Support managed service identities</span></span>
* <span data-ttu-id="77103-415">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="77103-415">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="77103-416">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="77103-416">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="77103-417">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="77103-417">May 10, 2017</span></span>

<span data-ttu-id="77103-418">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="77103-418">Version 2.0.6</span></span>

* <span data-ttu-id="77103-419">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="77103-419">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="77103-420">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="77103-420">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="77103-421">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="77103-421">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="77103-422">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="77103-422">Include Cognitive Services module.</span></span>
* <span data-ttu-id="77103-423">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="77103-423">Include Service Fabric module.</span></span>
* <span data-ttu-id="77103-424">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="77103-424">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="77103-425">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="77103-425">Add support for CDN commands.</span></span>
* <span data-ttu-id="77103-426">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="77103-426">Remove Container module.</span></span>
* <span data-ttu-id="77103-427">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="77103-427">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="77103-428">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77103-428">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="77103-429">Principal</span><span class="sxs-lookup"><span data-stu-id="77103-429">Core</span></span>

* <span data-ttu-id="77103-430">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="77103-430">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="77103-431">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="77103-431">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="77103-432">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="77103-432">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="77103-433">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="77103-433">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="77103-434">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="77103-434">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="77103-435">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="77103-435">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="77103-436">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="77103-436">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="77103-437">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="77103-437">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="77103-438">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="77103-438">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="77103-439">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="77103-439">core: Improved performance</span></span>
* <span data-ttu-id="77103-440">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="77103-440">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="77103-441">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="77103-441">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="77103-442">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-442">ACS</span></span>

* <span data-ttu-id="77103-443">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="77103-443">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="77103-444">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="77103-444">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="77103-445">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="77103-445">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="77103-446">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="77103-446">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="77103-447">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-447">AppService</span></span>

* <span data-ttu-id="77103-448">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="77103-448">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="77103-449">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="77103-449">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="77103-450">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="77103-450">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="77103-451">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="77103-451">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="77103-452">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="77103-452">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="77103-453">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="77103-453">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="77103-454">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="77103-454">support slot swap with preview</span></span>
* <span data-ttu-id="77103-455">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="77103-455">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="77103-456">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="77103-456">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77103-457">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77103-457">CosmosDB</span></span>

* <span data-ttu-id="77103-458">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="77103-458">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="77103-459">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="77103-459">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="77103-460">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="77103-460">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="77103-461">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="77103-461">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77103-462">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77103-462">Data Lake Analytics</span></span>

* <span data-ttu-id="77103-463">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="77103-463">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="77103-464">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="77103-464">Add support for new catalog item type: package.</span></span> <span data-ttu-id="77103-465">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="77103-465">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="77103-466">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="77103-466">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="77103-467">Table</span><span class="sxs-lookup"><span data-stu-id="77103-467">Table</span></span>
  * <span data-ttu-id="77103-468">Fonction table</span><span class="sxs-lookup"><span data-stu-id="77103-468">Table valued function</span></span>
  * <span data-ttu-id="77103-469">Affichage</span><span class="sxs-lookup"><span data-stu-id="77103-469">View</span></span>
  * <span data-ttu-id="77103-470">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="77103-470">Table Statistics.</span></span> <span data-ttu-id="77103-471">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="77103-471">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77103-472">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77103-472">Data Lake Store</span></span>

* <span data-ttu-id="77103-473">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="77103-473">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="77103-474">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77103-474">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="77103-475">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="77103-475">missed help for access show.</span></span> <span data-ttu-id="77103-476">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="77103-476">adding it.</span></span> <span data-ttu-id="77103-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="77103-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="77103-478">Rechercher</span><span class="sxs-lookup"><span data-stu-id="77103-478">Find</span></span>

* <span data-ttu-id="77103-479">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="77103-479">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="77103-480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77103-480">KeyVault</span></span>

* <span data-ttu-id="77103-481">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="77103-481">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="77103-482">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="77103-482">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="77103-483">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="77103-483">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="77103-484">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="77103-484">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="77103-485">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="77103-485">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="77103-486">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="77103-486">Lab</span></span>

* <span data-ttu-id="77103-487">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="77103-487">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="77103-488">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="77103-488">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="77103-489">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="77103-489">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="77103-490">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="77103-490">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="77103-491">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="77103-491">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="77103-492">Surveiller</span><span class="sxs-lookup"><span data-stu-id="77103-492">Monitor</span></span>

* <span data-ttu-id="77103-493">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="77103-493">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="77103-494">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="77103-494">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="77103-495">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-495">Network</span></span>

* <span data-ttu-id="77103-496">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="77103-496">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="77103-497">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="77103-497">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="77103-498">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="77103-498">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="77103-499">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="77103-499">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="77103-500">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="77103-500">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="77103-501">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="77103-501">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="77103-502">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="77103-502">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="77103-503">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="77103-503">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="77103-504">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="77103-504">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="77103-505">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="77103-505">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="77103-506">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="77103-506">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="77103-507">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="77103-507">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="77103-508">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="77103-508">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="77103-509">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="77103-509">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="77103-510">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="77103-510">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="77103-511">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="77103-511">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="77103-512">Profil</span><span class="sxs-lookup"><span data-stu-id="77103-512">Profile</span></span>

* <span data-ttu-id="77103-513">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="77103-513">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="77103-514">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="77103-514">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="77103-515">Redis</span><span class="sxs-lookup"><span data-stu-id="77103-515">Redis</span></span>

* <span data-ttu-id="77103-516">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="77103-516">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="77103-517">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="77103-517">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="77103-518">Ressource</span><span class="sxs-lookup"><span data-stu-id="77103-518">Resource</span></span>

* <span data-ttu-id="77103-519">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="77103-519">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="77103-520">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="77103-520">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="77103-521">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="77103-521">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="77103-522">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="77103-522">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="77103-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="77103-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="77103-524">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="77103-524">Add docs for az lock update.</span></span> <span data-ttu-id="77103-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="77103-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="77103-526">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="77103-526">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="77103-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="77103-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="77103-528">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="77103-528">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="77103-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="77103-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="77103-530">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="77103-530">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="77103-531">Rôle</span><span class="sxs-lookup"><span data-stu-id="77103-531">Role</span></span>

* <span data-ttu-id="77103-532">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="77103-532">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="77103-533">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="77103-533">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="77103-534">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="77103-534">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="77103-535">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="77103-535">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="77103-536">SQL</span><span class="sxs-lookup"><span data-stu-id="77103-536">SQL</span></span>

* <span data-ttu-id="77103-537">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="77103-537">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="77103-538">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="77103-538">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="77103-539">Storage</span><span class="sxs-lookup"><span data-stu-id="77103-539">Storage</span></span>

* <span data-ttu-id="77103-540">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="77103-540">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="77103-541">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="77103-541">Add support for incremental blob copy</span></span>
* <span data-ttu-id="77103-542">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="77103-542">Add support for large block blob upload</span></span>
* <span data-ttu-id="77103-543">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="77103-543">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="77103-544">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-544">VM</span></span>

* <span data-ttu-id="77103-545">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="77103-545">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="77103-546">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="77103-546">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="77103-547">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="77103-547">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="77103-548">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="77103-548">az vm/vmss disk</span></span>
  3. <span data-ttu-id="77103-549">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="77103-549">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="77103-550">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="77103-550">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="77103-551">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="77103-551">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="77103-552">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="77103-552">April 3, 2017</span></span>

<span data-ttu-id="77103-553">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="77103-553">Version 2.0.2</span></span>

<span data-ttu-id="77103-554">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="77103-554">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="77103-555">Principal</span><span class="sxs-lookup"><span data-stu-id="77103-555">Core</span></span>

* <span data-ttu-id="77103-556">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="77103-556">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="77103-557">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="77103-557">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="77103-558">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="77103-558">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="77103-559">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77103-559">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77103-560">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="77103-560">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="77103-561">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="77103-561">Add prompting for missing template parameters.</span></span> <span data-ttu-id="77103-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="77103-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="77103-563">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="77103-563">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="77103-564">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="77103-564">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="77103-565">ACS</span><span class="sxs-lookup"><span data-stu-id="77103-565">ACS</span></span>

* <span data-ttu-id="77103-566">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="77103-566">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="77103-567">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="77103-567">Add support for ssh key password prompting.</span></span> <span data-ttu-id="77103-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="77103-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="77103-569">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="77103-569">Add support for windows clusters.</span></span> <span data-ttu-id="77103-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="77103-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="77103-571">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="77103-571">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="77103-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="77103-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="77103-573">AppService</span><span class="sxs-lookup"><span data-stu-id="77103-573">AppService</span></span>

* <span data-ttu-id="77103-574">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="77103-574">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="77103-575">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="77103-575">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="77103-576">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="77103-576">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="77103-577">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="77103-577">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="77103-578">DataLake</span><span class="sxs-lookup"><span data-stu-id="77103-578">DataLake</span></span>

* <span data-ttu-id="77103-579">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="77103-579">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="77103-580">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="77103-580">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="77103-581">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="77103-581">DocuemntDB</span></span>

* <span data-ttu-id="77103-582">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="77103-582">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="77103-583">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="77103-583">VM</span></span>

* <span data-ttu-id="77103-584">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="77103-584">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="77103-585">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="77103-585">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="77103-586">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="77103-586">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="77103-587">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77103-587">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77103-588">Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="77103-588">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="77103-589">Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="77103-589">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="77103-590">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="77103-590">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="77103-591">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="77103-591">February 27, 2017</span></span>

<span data-ttu-id="77103-592">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="77103-592">Version 2.0.0</span></span>

<span data-ttu-id="77103-593">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="77103-593">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="77103-594">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="77103-594">General availability applies to these command modules:</span></span>
- <span data-ttu-id="77103-595">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="77103-595">Container Service (acs)</span></span>
- <span data-ttu-id="77103-596">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="77103-596">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="77103-597">Réseau</span><span class="sxs-lookup"><span data-stu-id="77103-597">Networking</span></span>
- <span data-ttu-id="77103-598">Stockage</span><span class="sxs-lookup"><span data-stu-id="77103-598">Storage</span></span>

<span data-ttu-id="77103-599">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="77103-599">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="77103-600">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="77103-600">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="77103-601">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="77103-601">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="77103-602">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="77103-602">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="77103-603">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="77103-603">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="77103-604">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="77103-604">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="77103-605">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="77103-605">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="77103-606">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="77103-606">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="77103-607">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="77103-607">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="77103-608">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="77103-608">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="77103-609">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="77103-609">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="77103-610">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="77103-610">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="77103-611">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="77103-611">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="77103-612">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="77103-612">Provide feedback from the command line with the `az feedback` command.</span></span>

