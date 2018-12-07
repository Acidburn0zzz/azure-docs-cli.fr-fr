---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/20/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7a2ab41dd6696d658d05ab76e44abf97626761aa
ms.sourcegitcommit: 14aa16beeec59e51890a6cba4906bdc8e19b94d0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/05/2018
ms.locfileid: "52892681"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="325f4-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="325f4-103">Azure CLI release notes</span></span>
## <a name="december-4-2018"></a><span data-ttu-id="325f4-104">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-104">December 4, 2018</span></span>

<span data-ttu-id="325f4-105">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="325f4-105">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="325f4-106">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-106">Core</span></span>
* <span data-ttu-id="325f4-107">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="325f4-107">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="325f4-108">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="325f4-108">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-109">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-109">Appservice</span></span>
* <span data-ttu-id="325f4-110">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="325f4-110">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="325f4-111">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="325f4-111">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="325f4-112">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-112">Network</span></span>
* <span data-ttu-id="325f4-113">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="325f4-113">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="325f4-114">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-114">Role</span></span>
* <span data-ttu-id="325f4-115">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="325f4-115">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="325f4-116">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-116">VM</span></span>
* <span data-ttu-id="325f4-117">[DÉCONSEILLÉ] Le paramètre `vm extension [show|wait] --expand` est déconseillé</span><span class="sxs-lookup"><span data-stu-id="325f4-117">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="325f4-118">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="325f4-118">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="325f4-119">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="325f4-119">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="325f4-120">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="325f4-120">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="325f4-121">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-121">November 20, 2018</span></span>

<span data-ttu-id="325f4-122">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="325f4-122">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="325f4-123">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-123">Core</span></span>
* <span data-ttu-id="325f4-124">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="325f4-124">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-125">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-125">ACR</span></span>
* <span data-ttu-id="325f4-126">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="325f4-126">Added context token to task step</span></span>
* <span data-ttu-id="325f4-127">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="325f4-127">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="325f4-128">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="325f4-128">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-129">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-129">Appservice</span></span>
* <span data-ttu-id="325f4-130">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="325f4-130">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="325f4-131">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="325f4-131">Updated the default `node_version`.</span></span> <span data-ttu-id="325f4-132">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="325f4-132">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="325f4-133">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="325f4-133">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="325f4-134">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="325f4-134">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="325f4-135">IotCentral</span><span class="sxs-lookup"><span data-stu-id="325f4-135">IotCentral</span></span>
* <span data-ttu-id="325f4-136">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="325f4-136">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-137">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-137">KeyVault</span></span>
* <span data-ttu-id="325f4-138">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="325f4-138">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="325f4-139">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-139">Network</span></span>
* <span data-ttu-id="325f4-140">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="325f4-140">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="325f4-141">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="325f4-141">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="325f4-142">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="325f4-142">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="325f4-143">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="325f4-143">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-144">Rdbms</span><span class="sxs-lookup"><span data-stu-id="325f4-144">Rdbms</span></span>
* <span data-ttu-id="325f4-145">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="325f4-145">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="325f4-146">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="325f4-146">Rbac</span></span>
* <span data-ttu-id="325f4-147">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="325f4-147">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="325f4-148">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="325f4-148">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="325f4-149">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-149">Storage</span></span>
* <span data-ttu-id="325f4-150">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-150">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="325f4-151">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="325f4-151">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="325f4-152">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="325f4-152">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="325f4-153">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="325f4-153">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-154">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-154">VM</span></span>
* <span data-ttu-id="325f4-155">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="325f4-155">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="325f4-156">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="325f4-156">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="325f4-157">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="325f4-157">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="325f4-158">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="325f4-158">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="325f4-159">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="325f4-159">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="325f4-160">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="325f4-160">Added `snapshot wait` command</span></span>
* <span data-ttu-id="325f4-161">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-161">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="325f4-162">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-162">November 6, 2018</span></span>

<span data-ttu-id="325f4-163">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="325f4-163">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="325f4-164">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-164">Core</span></span>
* <span data-ttu-id="325f4-165">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="325f4-165">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-166">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-166">ACR</span></span>
* <span data-ttu-id="325f4-167">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="325f4-167">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="325f4-168">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="325f4-168">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-169">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-169">ACS</span></span>
* <span data-ttu-id="325f4-170">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-170">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="325f4-171">Advisor</span><span class="sxs-lookup"><span data-stu-id="325f4-171">Advisor</span></span>
* <span data-ttu-id="325f4-172">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="325f4-172">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="325f4-173">AMS</span><span class="sxs-lookup"><span data-stu-id="325f4-173">AMS</span></span>
* <span data-ttu-id="325f4-174">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="325f4-174">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="325f4-175">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="325f4-175">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="325f4-176">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="325f4-176">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="325f4-177">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="325f4-177">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="325f4-178">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="325f4-178">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="325f4-179">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="325f4-179">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="325f4-180">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="325f4-180">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="325f4-181">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="325f4-181">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="325f4-182">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="325f4-182">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="325f4-183">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="325f4-183">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="325f4-184">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="325f4-184">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="325f4-185">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="325f4-185">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="325f4-186">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="325f4-186">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="325f4-187">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="325f4-187">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="325f4-188">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="325f4-188">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="325f4-189">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="325f4-189">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="325f4-190">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="325f4-190">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-191">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-191">AppService</span></span>
* <span data-ttu-id="325f4-192">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="325f4-192">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="325f4-193">Configuration</span><span class="sxs-lookup"><span data-stu-id="325f4-193">Configure</span></span>
* <span data-ttu-id="325f4-194">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="325f4-194">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="325f4-195">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-195">Container</span></span>
* <span data-ttu-id="325f4-196">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="325f4-196">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="325f4-197">Event Hub</span><span class="sxs-lookup"><span data-stu-id="325f4-197">EventHub</span></span>
* <span data-ttu-id="325f4-198">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-198">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-199">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-199">Interactive</span></span>
* <span data-ttu-id="325f4-200">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="325f4-200">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-201">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-201">Monitor</span></span>
* <span data-ttu-id="325f4-202">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-202">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="325f4-203">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-203">Network</span></span>
* <span data-ttu-id="325f4-204">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="325f4-204">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="325f4-205">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="325f4-205">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="325f4-206">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="325f4-206">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="325f4-207">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-207">Profile</span></span>
* <span data-ttu-id="325f4-208">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="325f4-208">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-209">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-209">RDBMS</span></span>
* <span data-ttu-id="325f4-210">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="325f4-210">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-211">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-211">Resource</span></span>
* <span data-ttu-id="325f4-212">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="325f4-212">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="325f4-213">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-213">Role</span></span>
* <span data-ttu-id="325f4-214">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="325f4-214">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="325f4-215">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="325f4-215">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="325f4-216">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="325f4-216">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-217">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-217">Storage</span></span>
* <span data-ttu-id="325f4-218">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="325f4-218">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-219">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-219">VM</span></span>
* <span data-ttu-id="325f4-220">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="325f4-220">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="325f4-221">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="325f4-221">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="325f4-222">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="325f4-222">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="325f4-223">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="325f4-223">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="325f4-224">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="325f4-224">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="325f4-225">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="325f4-225">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="325f4-226">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-226">October 23, 2018</span></span>

<span data-ttu-id="325f4-227">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="325f4-227">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="325f4-228">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-228">Core</span></span>
* <span data-ttu-id="325f4-229">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="325f4-229">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="325f4-230">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="325f4-230">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-231">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-231">ACR</span></span>
* <span data-ttu-id="325f4-232">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="325f4-232">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="325f4-233">CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-233">CDN</span></span>
* <span data-ttu-id="325f4-234">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="325f4-234">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="325f4-235">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="325f4-235">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="325f4-236">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-236">Container</span></span>
* <span data-ttu-id="325f4-237">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="325f4-237">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="325f4-238">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-238">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="325f4-239">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="325f4-239">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="325f4-240">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-240">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="325f4-241">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="325f4-241">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="325f4-242">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="325f4-242">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="325f4-243">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="325f4-243">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="325f4-244">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="325f4-244">CosmosDB</span></span>
* <span data-ttu-id="325f4-245">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="325f4-245">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-246">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-246">Interactive</span></span>
* <span data-ttu-id="325f4-247">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="325f4-247">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="325f4-248">IoT Central</span><span class="sxs-lookup"><span data-stu-id="325f4-248">IoT Central</span></span>
* <span data-ttu-id="325f4-249">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="325f4-249">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="325f4-250">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="325f4-250">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-251">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-251">Monitor</span></span>
* <span data-ttu-id="325f4-252">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="325f4-252">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="325f4-253">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-253">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="325f4-254">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="325f4-254">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="325f4-255">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="325f4-255">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="325f4-256">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="325f4-256">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="325f4-257">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="325f4-257">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="325f4-258">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="325f4-258">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="325f4-259">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="325f4-259">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="325f4-260">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="325f4-260">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="325f4-261">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="325f4-261">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="325f4-262">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-262">Network</span></span>
* <span data-ttu-id="325f4-263">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-263">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="325f4-264">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-264">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="325f4-265">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="325f4-265">ServiceBus</span></span>
* <span data-ttu-id="325f4-266">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="325f4-266">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-267">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-267">SQL</span></span>
* <span data-ttu-id="325f4-268">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="325f4-268">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-269">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-269">Storage</span></span>
* <span data-ttu-id="325f4-270">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="325f4-270">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="325f4-271">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="325f4-271">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-272">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-272">VM</span></span>
* <span data-ttu-id="325f4-273">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-273">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="325f4-274">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-274">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="325f4-275">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="325f4-275">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="325f4-276">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-276">October 16, 2018</span></span>

<span data-ttu-id="325f4-277">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="325f4-277">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-278">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-278">VM</span></span>
* <span data-ttu-id="325f4-279">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="325f4-279">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="325f4-280">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-280">October 9, 2018</span></span>

<span data-ttu-id="325f4-281">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="325f4-281">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="325f4-282">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-282">Core</span></span>
* <span data-ttu-id="325f4-283">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="325f4-283">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-284">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-284">ACR</span></span>
* <span data-ttu-id="325f4-285">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="325f4-285">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-286">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-286">ACS</span></span>
* <span data-ttu-id="325f4-287">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="325f4-287">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="325f4-288">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="325f4-288">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="325f4-289">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="325f4-289">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="325f4-290">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="325f4-290">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="325f4-291">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-291">Container</span></span>
* <span data-ttu-id="325f4-292">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="325f4-292">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="325f4-293">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-293">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="325f4-294">Event Hub</span><span class="sxs-lookup"><span data-stu-id="325f4-294">Event Hub</span></span>
* <span data-ttu-id="325f4-295">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="325f4-295">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="325f4-296">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="325f4-296">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="325f4-297">Extensions</span><span class="sxs-lookup"><span data-stu-id="325f4-297">Extensions</span></span>
* <span data-ttu-id="325f4-298">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="325f4-298">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="325f4-299">HDInsight</span><span class="sxs-lookup"><span data-stu-id="325f4-299">HDInsight</span></span>
* <span data-ttu-id="325f4-300">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-300">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-301">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-301">IoT</span></span>
* <span data-ttu-id="325f4-302">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="325f4-302">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-303">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-303">KeyVault</span></span>
* <span data-ttu-id="325f4-304">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="325f4-304">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="325f4-305">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-305">Network</span></span>
* <span data-ttu-id="325f4-306">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="325f4-306">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="325f4-307">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="325f4-307">See #6052</span></span>
* <span data-ttu-id="325f4-308">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="325f4-308">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="325f4-309">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="325f4-309">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="325f4-310">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="325f4-310">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="325f4-311">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="325f4-311">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="325f4-312">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="325f4-312">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="325f4-313">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="325f4-313">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="325f4-314">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-314">Role</span></span>
* <span data-ttu-id="325f4-315">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="325f4-315">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="325f4-316">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="325f4-316">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="325f4-317">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="325f4-317">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="325f4-318">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="325f4-318">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="325f4-319">Service Bus</span><span class="sxs-lookup"><span data-stu-id="325f4-319">Service Bus</span></span>
* <span data-ttu-id="325f4-320">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="325f4-320">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-321">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-321">VM</span></span>
* <span data-ttu-id="325f4-322">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="325f4-322">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="325f4-323">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="325f4-323">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="325f4-324">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="325f4-324">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="325f4-325">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="325f4-325">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="325f4-326">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="325f4-326">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="325f4-327">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="325f4-327">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="325f4-328">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-328">September 21, 2018</span></span>

<span data-ttu-id="325f4-329">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="325f4-329">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-330">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-330">ACR</span></span>
* <span data-ttu-id="325f4-331">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-331">Added ACR Task commands</span></span>
* <span data-ttu-id="325f4-332">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="325f4-332">Added quick run command</span></span>
* <span data-ttu-id="325f4-333">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="325f4-333">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="325f4-334">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-334">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="325f4-335">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="325f4-335">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="325f4-336">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="325f4-336">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-337">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-337">ACS</span></span>
* <span data-ttu-id="325f4-338">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-338">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="325f4-339">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="325f4-339">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-340">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-340">AppService</span></span>

* <span data-ttu-id="325f4-341">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="325f4-341">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="325f4-342">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="325f4-342">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="325f4-343">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="325f4-343">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="325f4-344">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="325f4-344">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-345">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-345">Batch</span></span>
* <span data-ttu-id="325f4-346">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="325f4-346">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="325f4-347">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="325f4-347">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="325f4-348">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="325f4-348">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="325f4-349">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="325f4-349">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="325f4-350">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-350">Batch AI</span></span> 
* <span data-ttu-id="325f4-351">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="325f4-351">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="325f4-352">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-352">Cognitive Services</span></span>
* <span data-ttu-id="325f4-353">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="325f4-353">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="325f4-354">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="325f4-354">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="325f4-355">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="325f4-355">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="325f4-356">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="325f4-356">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="325f4-357">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="325f4-357">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="325f4-358">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="325f4-358">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="325f4-359">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-359">Container</span></span>
* <span data-ttu-id="325f4-360">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="325f4-360">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="325f4-361">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-361">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="325f4-362">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="325f4-362">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="325f4-363">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-363">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="325f4-364">DataLake</span><span class="sxs-lookup"><span data-stu-id="325f4-364">Datalake</span></span>
* <span data-ttu-id="325f4-365">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="325f4-365">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="325f4-366">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="325f4-366">Interactive Shell</span></span>
* <span data-ttu-id="325f4-367">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-367">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="325f4-368">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="325f4-368">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-369">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-369">IoT</span></span>
* <span data-ttu-id="325f4-370">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-370">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="325f4-371">Key Vault</span><span class="sxs-lookup"><span data-stu-id="325f4-371">Key Vault</span></span>
* <span data-ttu-id="325f4-372">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="325f4-372">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="325f4-373">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-373">Network</span></span>
* <span data-ttu-id="325f4-374">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="325f4-374">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="325f4-375">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="325f4-375">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="325f4-376">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="325f4-376">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="325f4-377">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="325f4-377">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="325f4-378">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="325f4-378">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="325f4-379">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="325f4-379">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="325f4-380">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="325f4-380">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="325f4-381">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="325f4-381">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="325f4-382">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="325f4-382">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="325f4-383">`network express-route create/update` : ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="325f4-383">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="325f4-384">`network vnet subnet create/update` : ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="325f4-384">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="325f4-385">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="325f4-385">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="325f4-386">`network traffic-manager profile create/update` : ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="325f4-386">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="325f4-387">`network lb frontend-ip create/update` : correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="325f4-387">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="325f4-388">`dns record-set * create/update` : ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="325f4-388">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="325f4-389">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="325f4-389">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="325f4-390">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-390">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="325f4-391">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="325f4-391">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-392">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-392">RDBMS</span></span>
* <span data-ttu-id="325f4-393">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="325f4-393">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="325f4-394">Réservation</span><span class="sxs-lookup"><span data-stu-id="325f4-394">Reservation</span></span>
* <span data-ttu-id="325f4-395">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="325f4-395">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="325f4-396">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="325f4-396">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="325f4-397">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="325f4-397">Manage App</span></span>
* <span data-ttu-id="325f4-398">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="325f4-398">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="325f4-399">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="325f4-399">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="325f4-400">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-400">Role</span></span>
* <span data-ttu-id="325f4-401">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="325f4-401">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="325f4-402">SignalR</span><span class="sxs-lookup"><span data-stu-id="325f4-402">SignalR</span></span>
* <span data-ttu-id="325f4-403">Première version</span><span class="sxs-lookup"><span data-stu-id="325f4-403">First release</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-404">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-404">Storage</span></span>
* <span data-ttu-id="325f4-405">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="325f4-405">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="325f4-406">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="325f4-406">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-407">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-407">VM</span></span>
* <span data-ttu-id="325f4-408">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="325f4-408">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="325f4-409">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="325f4-409">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="325f4-410">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-410">August 28, 2018</span></span>

<span data-ttu-id="325f4-411">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="325f4-411">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="325f4-412">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-412">Core</span></span>

* <span data-ttu-id="325f4-413">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="325f4-413">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="325f4-414">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="325f4-414">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-415">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-415">ACR</span></span>

* <span data-ttu-id="325f4-416">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="325f4-416">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="325f4-417">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="325f4-417">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-418">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-418">ACS</span></span>

* <span data-ttu-id="325f4-419">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="325f4-419">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="325f4-420">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="325f4-420">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-421">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-421">AppService</span></span>

* <span data-ttu-id="325f4-422">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="325f4-422">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="325f4-423">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="325f4-423">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="325f4-424">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-424">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="325f4-425">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="325f4-425">Backup</span></span>

* <span data-ttu-id="325f4-426">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-426">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="325f4-427">Service de robot</span><span class="sxs-lookup"><span data-stu-id="325f4-427">Bot Service</span></span>

* <span data-ttu-id="325f4-428">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="325f4-428">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="325f4-429">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-429">Cognitive Services</span></span>

* <span data-ttu-id="325f4-430">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="325f4-430">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-431">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-431">IoT</span></span>

* <span data-ttu-id="325f4-432">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="325f4-432">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-433">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-433">Monitor</span></span>

* <span data-ttu-id="325f4-434">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="325f4-434">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="325f4-435">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="325f4-435">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="325f4-436">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-436">Network</span></span>

* <span data-ttu-id="325f4-437">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-437">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-438">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-438">Resource</span></span>

* <span data-ttu-id="325f4-439">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-439">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-440">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-440">Storage</span></span>

* <span data-ttu-id="325f4-441">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-441">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-442">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-442">VM</span></span>

* <span data-ttu-id="325f4-443">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-443">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="325f4-444">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-444">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="325f4-445">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-445">Auguest 14, 2018</span></span>

<span data-ttu-id="325f4-446">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="325f4-446">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="325f4-447">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-447">Core</span></span>

* <span data-ttu-id="325f4-448">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="325f4-448">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="325f4-449">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="325f4-449">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="325f4-450">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="325f4-450">Telemetry</span></span>

* <span data-ttu-id="325f4-451">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="325f4-451">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-452">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-452">ACR</span></span>

* <span data-ttu-id="325f4-453">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="325f4-453">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="325f4-454">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="325f4-454">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-455">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-455">ACS</span></span>

* <span data-ttu-id="325f4-456">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-456">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="325f4-457">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-457">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="325f4-458">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="325f4-458">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="325f4-459">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="325f4-459">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="325f4-460">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="325f4-460">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="325f4-461">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-461">AppService</span></span>

* <span data-ttu-id="325f4-462">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="325f4-462">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="325f4-463">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="325f4-463">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="325f4-464">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-464">BatchAI</span></span>

* <span data-ttu-id="325f4-465">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="325f4-465">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="325f4-466">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-466">Container</span></span>

* <span data-ttu-id="325f4-467">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-467">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="325f4-468">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-468">IoT</span></span>

* <span data-ttu-id="325f4-469">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="325f4-469">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="325f4-470">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="325f4-470">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="325f4-471">Iot Central</span><span class="sxs-lookup"><span data-stu-id="325f4-471">Iot Central</span></span>

* <span data-ttu-id="325f4-472">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="325f4-472">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-473">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-473">KeyVault</span></span>


* <span data-ttu-id="325f4-474">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="325f4-474">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="325f4-475">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-475">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="325f4-476">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="325f4-476">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="325f4-477">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="325f4-477">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="325f4-478">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="325f4-478">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="325f4-479">Relais</span><span class="sxs-lookup"><span data-stu-id="325f4-479">Relay</span></span>

* <span data-ttu-id="325f4-480">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-480">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-481">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-481">Sql</span></span>

* <span data-ttu-id="325f4-482">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="325f4-482">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-483">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-483">Storage</span></span>

* <span data-ttu-id="325f4-484">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="325f4-484">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="325f4-485">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="325f4-485">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="325f4-486">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="325f4-486">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="325f4-487">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="325f4-487">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="325f4-488">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-488">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-489">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-489">VM</span></span>

* <span data-ttu-id="325f4-490">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="325f4-490">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="325f4-491">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-491">July 31, 2018</span></span>

<span data-ttu-id="325f4-492">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="325f4-492">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-493">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-493">ACR</span></span>

* <span data-ttu-id="325f4-494">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="325f4-494">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="325f4-495">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="325f4-495">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-496">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-496">ACS</span></span>

* <span data-ttu-id="325f4-497">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="325f4-497">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-498">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-498">Batch</span></span>

* <span data-ttu-id="325f4-499">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="325f4-499">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="325f4-500">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-500">Container</span></span>

* <span data-ttu-id="325f4-501">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="325f4-501">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="325f4-502">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-502">Network</span></span>

* <span data-ttu-id="325f4-503">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="325f4-503">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="325f4-504">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-504">Resource</span></span>

* <span data-ttu-id="325f4-505">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="325f4-505">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="325f4-506">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="325f4-506">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="325f4-507">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-507">Role</span></span>

* <span data-ttu-id="325f4-508">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="325f4-508">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="325f4-509">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-509">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="325f4-510">Recherche</span><span class="sxs-lookup"><span data-stu-id="325f4-510">Search</span></span>

* <span data-ttu-id="325f4-511">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="325f4-511">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="325f4-512">Service Bus</span><span class="sxs-lookup"><span data-stu-id="325f4-512">Service Bus</span></span>

* <span data-ttu-id="325f4-513">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="325f4-513">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="325f4-514">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-514">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="325f4-515">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="325f4-515">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="325f4-516">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="325f4-516">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-517">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-517">Storage</span></span>

* <span data-ttu-id="325f4-518">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="325f4-518">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="325f4-519">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-519">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-520">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-520">VM</span></span>

* <span data-ttu-id="325f4-521">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-521">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="325f4-522">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="325f4-522">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="325f4-523">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="325f4-523">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="325f4-524">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="325f4-524">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="325f4-525">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-525">July 18, 2018</span></span>

<span data-ttu-id="325f4-526">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="325f4-526">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="325f4-527">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-527">Core</span></span>

* <span data-ttu-id="325f4-528">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="325f4-528">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="325f4-529">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="325f4-529">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="325f4-530">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="325f4-530">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-531">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-531">ACR</span></span>

* <span data-ttu-id="325f4-532">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="325f4-532">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="325f4-533">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="325f4-533">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="325f4-534">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="325f4-534">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="325f4-535">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="325f4-535">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-536">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-536">ACS</span></span>

* <span data-ttu-id="325f4-537">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="325f4-537">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-538">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-538">AppService</span></span>

* <span data-ttu-id="325f4-539">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="325f4-539">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-540">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-540">Batch</span></span>

* <span data-ttu-id="325f4-541">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="325f4-541">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="325f4-542">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="325f4-542">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="325f4-543">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-543">Batch AI</span></span>

* <span data-ttu-id="325f4-544">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="325f4-544">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="325f4-545">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-545">Container</span></span>

* <span data-ttu-id="325f4-546">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="325f4-546">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="325f4-547">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="325f4-547">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="325f4-548">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-548">Network</span></span>

* <span data-ttu-id="325f4-549">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="325f4-549">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="325f4-550">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="325f4-550">Added `network nic wait`</span></span>
* <span data-ttu-id="325f4-551">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="325f4-551">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="325f4-552">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="325f4-552">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="325f4-553">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-553">Resource</span></span>

* <span data-ttu-id="325f4-554">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="325f4-554">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="325f4-555">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="325f4-555">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="325f4-556">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="325f4-556">Added `deployment wait` command</span></span>
* <span data-ttu-id="325f4-557">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="325f4-557">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-558">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-558">SQL</span></span>

* <span data-ttu-id="325f4-559">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="325f4-559">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="325f4-560">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="325f4-560">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="325f4-561">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="325f4-561">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-562">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-562">Storage</span></span>

* <span data-ttu-id="325f4-563">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="325f4-563">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-564">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-564">VM</span></span>

* <span data-ttu-id="325f4-565">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-565">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="325f4-566">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="325f4-566">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="325f4-567">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="325f4-567">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="325f4-568">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-568">July 3, 2018</span></span>

<span data-ttu-id="325f4-569">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="325f4-569">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="325f4-570">AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-570">AKS</span></span>

* <span data-ttu-id="325f4-571">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-571">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="325f4-572">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-572">July 3, 2018</span></span>

<span data-ttu-id="325f4-573">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="325f4-573">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="325f4-574">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-574">Core</span></span>

* <span data-ttu-id="325f4-575">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-575">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-576">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-576">ACR</span></span>

* <span data-ttu-id="325f4-577">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="325f4-577">Added polling build status</span></span>
* <span data-ttu-id="325f4-578">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="325f4-578">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="325f4-579">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="325f4-579">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-580">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-580">ACS</span></span>

* <span data-ttu-id="325f4-581">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-581">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="325f4-582">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-582">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="325f4-583">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="325f4-583">Updated options for `aks browse` command.</span></span> <span data-ttu-id="325f4-584">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="325f4-584">Added `--listen-port` support</span></span>
* <span data-ttu-id="325f4-585">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="325f4-585">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="325f4-586">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="325f4-586">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="325f4-587">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="325f4-587">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-588">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-588">AppService</span></span>

* <span data-ttu-id="325f4-589">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="325f4-589">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="325f4-590">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="325f4-590">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="325f4-591">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="325f4-591">Backup</span></span>

* <span data-ttu-id="325f4-592">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="325f4-592">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="325f4-593">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-593">BatchAI</span></span>

* <span data-ttu-id="325f4-594">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="325f4-594">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="325f4-595">Cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-595">Cloud</span></span>

* <span data-ttu-id="325f4-596">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-596">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="325f4-597">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-597">Container</span></span>

* <span data-ttu-id="325f4-598">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="325f4-598">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="325f4-599">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="325f4-599">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="325f4-600">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="325f4-600">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-601">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-601">Extension</span></span>

* <span data-ttu-id="325f4-602">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="325f4-602">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="325f4-603">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-603">Network</span></span>

* <span data-ttu-id="325f4-604">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="325f4-604">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-605">Rdbms</span><span class="sxs-lookup"><span data-stu-id="325f4-605">Rdbms</span></span>

* <span data-ttu-id="325f4-606">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="325f4-606">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-607">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-607">Resource</span></span>

* <span data-ttu-id="325f4-608">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="325f4-608">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-609">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-609">VM</span></span>

* <span data-ttu-id="325f4-610">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="325f4-610">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="325f4-611">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-611">June 25, 2018</span></span>

<span data-ttu-id="325f4-612">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="325f4-612">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="325f4-613">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-613">CLI</span></span>

* <span data-ttu-id="325f4-614">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="325f4-614">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="325f4-615">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-615">June 19, 2018</span></span>

<span data-ttu-id="325f4-616">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="325f4-616">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="325f4-617">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-617">Core</span></span>

* <span data-ttu-id="325f4-618">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-618">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-619">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-619">ACR</span></span>

* <span data-ttu-id="325f4-620">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="325f4-620">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="325f4-621">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="325f4-621">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-622">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-622">ACS</span></span>

* <span data-ttu-id="325f4-623">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="325f4-623">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="325f4-624">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="325f4-624">Added `--update` support</span></span>
* <span data-ttu-id="325f4-625">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="325f4-625">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="325f4-626">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="325f4-626">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="325f4-627">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="325f4-627">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="325f4-628">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="325f4-628">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="325f4-629">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="325f4-629">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="325f4-630">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="325f4-630">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-631">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-631">AppService</span></span>

* <span data-ttu-id="325f4-632">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="325f4-632">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="325f4-633">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="325f4-633">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-634">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-634">Batch</span></span>

* <span data-ttu-id="325f4-635">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="325f4-635">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="325f4-636">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-636">Batch AI</span></span>

* <span data-ttu-id="325f4-637">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="325f4-637">Added support for workspaces.</span></span> <span data-ttu-id="325f4-638">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="325f4-638">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="325f4-639">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="325f4-639">Added support for experiments.</span></span> <span data-ttu-id="325f4-640">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="325f4-640">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="325f4-641">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="325f4-641">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="325f4-642">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="325f4-642">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="325f4-643">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="325f4-643">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="325f4-644">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="325f4-644">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="325f4-645">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="325f4-645">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="325f4-646">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="325f4-646">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="325f4-647">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="325f4-647">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="325f4-648">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="325f4-648">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="325f4-649">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="325f4-649">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="325f4-650">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="325f4-650">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="325f4-651">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="325f4-651">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="325f4-652">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="325f4-652">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="325f4-653">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="325f4-653">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="325f4-654">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="325f4-654">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="325f4-655">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="325f4-655">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="325f4-656">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="325f4-656">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="325f4-657">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="325f4-657">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="325f4-658">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="325f4-658">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="325f4-659">Cartes</span><span class="sxs-lookup"><span data-stu-id="325f4-659">Maps</span></span>

* <span data-ttu-id="325f4-660">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="325f4-660">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="325f4-661">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-661">Network</span></span>

* <span data-ttu-id="325f4-662">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="325f4-662">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="325f4-663">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="325f4-663">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="325f4-664">#6502</span><span class="sxs-lookup"><span data-stu-id="325f4-664">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="325f4-665">Réservations</span><span class="sxs-lookup"><span data-stu-id="325f4-665">Reservations</span></span>

* <span data-ttu-id="325f4-666">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="325f4-666">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="325f4-667">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="325f4-667">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="325f4-668">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="325f4-668">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="325f4-669">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="325f4-669">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="325f4-670">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="325f4-670">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="325f4-671">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="325f4-671">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="325f4-672">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-672">Role</span></span>

* <span data-ttu-id="325f4-673">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="325f4-673">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-674">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-674">SQL</span></span>

* <span data-ttu-id="325f4-675">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-675">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-676">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-676">Storage</span></span>

* <span data-ttu-id="325f4-677">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="325f4-677">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-678">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-678">VM</span></span>

* <span data-ttu-id="325f4-679">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-679">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="325f4-680">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="325f4-680">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="325f4-681">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="325f4-681">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="325f4-682">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-682">June 13, 2018</span></span>

<span data-ttu-id="325f4-683">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="325f4-683">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="325f4-684">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-684">Core</span></span>

* <span data-ttu-id="325f4-685">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-685">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="325f4-686">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-686">June 13, 2018</span></span>

<span data-ttu-id="325f4-687">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="325f4-687">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="325f4-688">AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-688">AKS</span></span>

* <span data-ttu-id="325f4-689">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="325f4-689">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="325f4-690">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="325f4-690">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="325f4-691">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="325f4-691">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="325f4-692">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="325f4-692">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="325f4-693">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="325f4-693">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-694">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-694">AppService</span></span>

* <span data-ttu-id="325f4-695">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="325f4-695">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="325f4-696">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-696">June 5, 2018</span></span>

<span data-ttu-id="325f4-697">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="325f4-697">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-698">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-698">Interactive</span></span>

* <span data-ttu-id="325f4-699">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="325f4-699">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="325f4-700">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-700">June 5, 2018</span></span>

<span data-ttu-id="325f4-701">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="325f4-701">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="325f4-702">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-702">Core</span></span>

* <span data-ttu-id="325f4-703">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="325f4-703">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="325f4-704">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="325f4-704">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-705">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-705">ACR</span></span>

* <span data-ttu-id="325f4-706">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="325f4-706">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="325f4-707">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="325f4-707">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="325f4-708">AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-708">AKS</span></span>

* <span data-ttu-id="325f4-709">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="325f4-709">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-710">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-710">Batch</span></span>

* <span data-ttu-id="325f4-711">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="325f4-711">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-712">IOT</span><span class="sxs-lookup"><span data-stu-id="325f4-712">IOT</span></span>

* <span data-ttu-id="325f4-713">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="325f4-713">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="325f4-714">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-714">Network</span></span>

* <span data-ttu-id="325f4-715">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="325f4-715">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="325f4-716">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="325f4-716">Policy Insights</span></span>

* <span data-ttu-id="325f4-717">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-717">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="325f4-718">ARM</span><span class="sxs-lookup"><span data-stu-id="325f4-718">ARM</span></span>

* <span data-ttu-id="325f4-719">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="325f4-719">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-720">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-720">SQL</span></span>

* <span data-ttu-id="325f4-721">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="325f4-721">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="325f4-722">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="325f4-722">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="325f4-723">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-723">Storage</span></span>

* <span data-ttu-id="325f4-724">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="325f4-724">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-725">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-725">VM</span></span>

* <span data-ttu-id="325f4-726">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="325f4-726">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="325f4-727">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-727">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="325f4-728">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="325f4-728">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="325f4-729">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-729">May 22, 2018</span></span>

<span data-ttu-id="325f4-730">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="325f4-730">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="325f4-731">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-731">Core</span></span>

* <span data-ttu-id="325f4-732">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="325f4-732">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-733">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-733">ACS</span></span>

* <span data-ttu-id="325f4-734">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="325f4-734">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="325f4-735">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="325f4-735">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-736">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-736">AppService</span></span>

* <span data-ttu-id="325f4-737">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="325f4-737">Improved generic update commands</span></span>
* <span data-ttu-id="325f4-738">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="325f4-738">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="325f4-739">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-739">Container</span></span>

* <span data-ttu-id="325f4-740">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="325f4-740">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="325f4-741">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-741">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-742">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-742">Extension</span></span>

* <span data-ttu-id="325f4-743">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="325f4-743">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-744">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-744">Interactive</span></span>

* <span data-ttu-id="325f4-745">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="325f4-745">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="325f4-746">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="325f4-746">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-747">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-747">KeyVault</span></span>

* <span data-ttu-id="325f4-748">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="325f4-748">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="325f4-749">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-749">Network</span></span>

* <span data-ttu-id="325f4-750">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="325f4-750">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="325f4-751">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="325f4-751">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-752">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-752">SQL</span></span>

* <span data-ttu-id="325f4-753">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="325f4-753">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="325f4-754">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="325f4-754">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="325f4-755">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="325f4-755">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="325f4-756">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="325f4-756">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="325f4-757">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="325f4-757">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="325f4-758">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="325f4-758">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="325f4-759">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="325f4-759">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="325f4-760">`edition`.</span><span class="sxs-lookup"><span data-stu-id="325f4-760">`edition`.</span></span> <span data-ttu-id="325f4-761">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="325f4-761">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="325f4-762">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="325f4-762">`elasticPoolName`.</span></span> <span data-ttu-id="325f4-763">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="325f4-763">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="325f4-764">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="325f4-764">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="325f4-765">`edition`.</span><span class="sxs-lookup"><span data-stu-id="325f4-765">`edition`.</span></span> <span data-ttu-id="325f4-766">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="325f4-766">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="325f4-767">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="325f4-767">`dtu`.</span></span> <span data-ttu-id="325f4-768">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="325f4-768">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="325f4-769">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="325f4-769">`databaseDtuMin`.</span></span> <span data-ttu-id="325f4-770">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="325f4-770">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="325f4-771">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="325f4-771">`databaseDtuMax`.</span></span> <span data-ttu-id="325f4-772">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="325f4-772">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="325f4-773">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="325f4-773">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="325f4-774">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="325f4-774">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-775">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-775">Storage</span></span>

* <span data-ttu-id="325f4-776">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-776">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="325f4-777">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="325f4-777">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-778">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-778">VM</span></span>

* <span data-ttu-id="325f4-779">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="325f4-779">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="325f4-780">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="325f4-780">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="325f4-781">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="325f4-781">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="325f4-782">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="325f4-782">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="325f4-783">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="325f4-783">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="325f4-784">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-784">May 7, 2018</span></span>

<span data-ttu-id="325f4-785">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="325f4-785">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="325f4-786">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-786">Core</span></span>

* <span data-ttu-id="325f4-787">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="325f4-787">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="325f4-788">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="325f4-788">Added limited support for positional arguments</span></span>
* <span data-ttu-id="325f4-789">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="325f4-789">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="325f4-790">#5591</span><span class="sxs-lookup"><span data-stu-id="325f4-790">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="325f4-791">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="325f4-791">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="325f4-792">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="325f4-792">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="325f4-793">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-793">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="325f4-794">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="325f4-794">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="325f4-795">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-795">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-796">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-796">ACR</span></span>

* <span data-ttu-id="325f4-797">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-797">Added ACR Build commands</span></span>
* <span data-ttu-id="325f4-798">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="325f4-798">Improved resource not found error messages</span></span>
* <span data-ttu-id="325f4-799">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="325f4-799">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="325f4-800">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="325f4-800">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="325f4-801">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="325f4-801">Improved repository commands error messages</span></span>
* <span data-ttu-id="325f4-802">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="325f4-802">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-803">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-803">ACS</span></span>

* <span data-ttu-id="325f4-804">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="325f4-804">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="325f4-805">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="325f4-805">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="325f4-806">AMS</span><span class="sxs-lookup"><span data-stu-id="325f4-806">AMS</span></span>

* <span data-ttu-id="325f4-807">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="325f4-807">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-808">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-808">Appservice</span></span>

* <span data-ttu-id="325f4-809">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="325f4-809">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="325f4-810">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="325f4-810">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="325f4-811">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="325f4-811">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="325f4-812">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-812">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="325f4-813">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-813">Batch AI</span></span>

* <span data-ttu-id="325f4-814">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="325f4-814">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="325f4-815">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-815">Cognitive Services</span></span>

* <span data-ttu-id="325f4-816">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="325f4-816">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="325f4-817">Consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-817">Consumption</span></span>

* <span data-ttu-id="325f4-818">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="325f4-818">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="325f4-819">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-819">Container</span></span>

* <span data-ttu-id="325f4-820">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="325f4-820">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="325f4-821">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="325f4-821">Cosmos DB</span></span>

* <span data-ttu-id="325f4-822">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="325f4-822">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="325f4-823">DMS</span><span class="sxs-lookup"><span data-stu-id="325f4-823">DMS</span></span>

* <span data-ttu-id="325f4-824">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="325f4-824">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-825">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-825">Extension</span></span>

* <span data-ttu-id="325f4-826">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="325f4-826">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-827">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-827">Interactive</span></span>

* <span data-ttu-id="325f4-828">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="325f4-828">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="325f4-829">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="325f4-829">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="325f4-830">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="325f4-830">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="325f4-831">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-831">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="325f4-832">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-832">Lab</span></span>

* <span data-ttu-id="325f4-833">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="325f4-833">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="325f4-834">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-834">Network</span></span>

* <span data-ttu-id="325f4-835">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="325f4-835">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="325f4-836">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-836">Profile</span></span>

* <span data-ttu-id="325f4-837">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="325f4-837">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="325f4-838">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="325f4-838">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="325f4-839">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="325f4-839">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="325f4-840">Redis</span><span class="sxs-lookup"><span data-stu-id="325f4-840">Redis</span></span>

* <span data-ttu-id="325f4-841">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="325f4-841">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="325f4-842">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="325f4-842">Deprecated `redis list-all`.</span></span> <span data-ttu-id="325f4-843">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="325f4-843">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="325f4-844">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="325f4-844">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="325f4-845">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-845">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="325f4-846">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-846">Role</span></span>

* <span data-ttu-id="325f4-847">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="325f4-847">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-848">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-848">Storage</span></span>

* <span data-ttu-id="325f4-849">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="325f4-849">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="325f4-850">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="325f4-850">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="325f4-851">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="325f4-851">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="325f4-852">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="325f4-852">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="325f4-853">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="325f4-853">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-854">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-854">VM</span></span>

* <span data-ttu-id="325f4-855">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="325f4-855">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="325f4-856">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="325f4-856">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="325f4-857">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="325f4-857">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="325f4-858">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="325f4-858">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="325f4-859">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="325f4-859">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="325f4-860">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="325f4-860">Added write accelerator support</span></span>
* <span data-ttu-id="325f4-861">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="325f4-861">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="325f4-862">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-862">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="325f4-863">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="325f4-863">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="325f4-864">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-864">April 10, 2018</span></span>

<span data-ttu-id="325f4-865">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="325f4-865">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-866">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-866">ACR</span></span>

* <span data-ttu-id="325f4-867">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="325f4-867">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-868">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-868">ACS</span></span>

* <span data-ttu-id="325f4-869">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="325f4-869">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-870">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-870">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="325f4-872">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="325f4-872">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="325f4-873">Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-873">BatchAI</span></span>

* <span data-ttu-id="325f4-874">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="325f4-874">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="325f4-875">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="325f4-875">Job level mounting</span></span>
  - <span data-ttu-id="325f4-876">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="325f4-876">Environment variables with secret values</span></span>
  - <span data-ttu-id="325f4-877">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="325f4-877">Performance counters settings</span></span>
  - <span data-ttu-id="325f4-878">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="325f4-878">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="325f4-879">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="325f4-879">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="325f4-880">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="325f4-880">Usage and limits reporting</span></span>
  - <span data-ttu-id="325f4-881">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="325f4-881">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="325f4-882">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="325f4-882">Support for custom images</span></span>
  - <span data-ttu-id="325f4-883">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="325f4-883">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="325f4-884">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="325f4-884">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="325f4-885">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="325f4-885">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="325f4-886">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="325f4-886">National clouds are supported</span></span>
* <span data-ttu-id="325f4-887">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="325f4-887">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="325f4-888">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="325f4-888">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="325f4-889">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-889">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="325f4-890">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="325f4-890">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="325f4-891">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="325f4-891">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="325f4-892">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="325f4-892">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="325f4-893">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="325f4-893">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="325f4-894">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="325f4-894">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="325f4-895">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="325f4-895">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="325f4-896">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="325f4-896">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="325f4-897">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-897">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="325f4-898">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="325f4-898">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="325f4-899">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="325f4-899">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="325f4-900">Facturation</span><span class="sxs-lookup"><span data-stu-id="325f4-900">Billing</span></span>

* <span data-ttu-id="325f4-901">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="325f4-901">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="325f4-902">Consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-902">Consumption</span></span>

* <span data-ttu-id="325f4-903">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="325f4-903">Added `marketplace` commands</span></span>
* <span data-ttu-id="325f4-904">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="325f4-904">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="325f4-905">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="325f4-905">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="325f4-906">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="325f4-906">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="325f4-907">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="325f4-907">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="325f4-908">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="325f4-908">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="325f4-909">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-909">Container</span></span>

* <span data-ttu-id="325f4-910">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="325f4-910">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="325f4-911">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="325f4-911">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-912">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-912">Extension</span></span>

* <span data-ttu-id="325f4-913">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="325f4-913">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-914">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-914">Interactive</span></span>

* <span data-ttu-id="325f4-915">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="325f4-915">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="325f4-916">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-916">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="325f4-917">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="325f4-917">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="325f4-918">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-918">Network</span></span>

* <span data-ttu-id="325f4-919">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="325f4-919">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="325f4-920">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="325f4-920">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="325f4-921">#4910</span><span class="sxs-lookup"><span data-stu-id="325f4-921">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="325f4-922">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="325f4-922">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="325f4-923">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="325f4-923">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="325f4-924">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-924">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="325f4-925">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-925">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="325f4-926">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="325f4-926">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-927">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-927">Profile</span></span>

* <span data-ttu-id="325f4-928">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="325f4-928">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="325f4-929">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="325f4-929">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-930">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-930">RDBMS</span></span>

* <span data-ttu-id="325f4-931">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="325f4-931">Added `georestore` command</span></span>
* <span data-ttu-id="325f4-932">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="325f4-932">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-933">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-933">Resource</span></span>

* <span data-ttu-id="325f4-934">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="325f4-934">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="325f4-935">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="325f4-935">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-936">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-936">SQL</span></span>

* <span data-ttu-id="325f4-937">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="325f4-937">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-938">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-938">Storage</span></span>

* <span data-ttu-id="325f4-939">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="325f4-939">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-940">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-940">VM</span></span>

* <span data-ttu-id="325f4-941">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="325f4-941">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="325f4-942">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="325f4-942">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="325f4-944">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-944">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="325f4-945">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="325f4-945">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="325f4-946">#5718</span><span class="sxs-lookup"><span data-stu-id="325f4-946">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="325f4-947">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="325f4-947">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="325f4-948">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-948">March 27, 2018</span></span>

<span data-ttu-id="325f4-949">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="325f4-949">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="325f4-950">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-950">Core</span></span>

* <span data-ttu-id="325f4-951">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="325f4-951">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-952">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-952">ACS</span></span>

* <span data-ttu-id="325f4-953">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="325f4-953">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-954">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-954">Appservice</span></span>

* <span data-ttu-id="325f4-955">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="325f4-955">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="325f4-956">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="325f4-956">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="325f4-957">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="325f4-957">Backup</span></span>

* <span data-ttu-id="325f4-958">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="325f4-958">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="325f4-959">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-959">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="325f4-960">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="325f4-960">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="325f4-961">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="325f4-961">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="325f4-962">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-962">Container</span></span>

* <span data-ttu-id="325f4-963">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="325f4-963">Added `container exec` command.</span></span> <span data-ttu-id="325f4-964">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="325f4-964">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="325f4-965">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-965">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-966">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-966">Extension</span></span>

* <span data-ttu-id="325f4-967">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="325f4-967">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="325f4-968">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="325f4-968">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="325f4-969">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-969">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-970">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-970">Interactive</span></span>

* <span data-ttu-id="325f4-971">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-971">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="325f4-972">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="325f4-972">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="325f4-973">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="325f4-973">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="325f4-974">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="325f4-974">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="325f4-975">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-975">Lab</span></span>

* <span data-ttu-id="325f4-976">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="325f4-976">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-977">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-977">Monitor</span></span>

* <span data-ttu-id="325f4-978">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="325f4-978">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="325f4-979">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="325f4-979">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="325f4-980">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="325f4-980">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="325f4-981">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-981">Network</span></span>

* <span data-ttu-id="325f4-982">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="325f4-982">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-983">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-983">Profile</span></span>

* <span data-ttu-id="325f4-984">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="325f4-984">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-985">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-985">RDBMS</span></span>

* <span data-ttu-id="325f4-986">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="325f4-986">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-987">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-987">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="325f4-989">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-989">Role</span></span>

* <span data-ttu-id="325f4-990">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="325f4-990">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="325f4-991">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="325f4-991">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="325f4-992">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="325f4-992">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="325f4-993">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="325f4-993">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="325f4-994">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="325f4-994">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-995">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-995">Storage</span></span>

* <span data-ttu-id="325f4-996">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="325f4-996">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="325f4-997">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="325f4-997">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-998">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-998">VM</span></span>

* <span data-ttu-id="325f4-999">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="325f4-999">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="325f4-1000">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1000">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="325f4-1001">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="325f4-1001">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="325f4-1002">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="325f4-1002">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="325f4-1003">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-1003">March 13, 2018</span></span>

<span data-ttu-id="325f4-1004">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="325f4-1004">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-1005">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1005">ACR</span></span>

* <span data-ttu-id="325f4-1006">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="325f4-1006">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="325f4-1007">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="325f4-1007">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="325f4-1008">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="325f4-1008">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1009">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1009">ACS</span></span>

* <span data-ttu-id="325f4-1010">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="325f4-1010">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="325f4-1011">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="325f4-1011">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="325f4-1012">Advisor</span><span class="sxs-lookup"><span data-stu-id="325f4-1012">Advisor</span></span>

* <span data-ttu-id="325f4-1013">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="325f4-1013">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="325f4-1014">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1014">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="325f4-1015">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="325f4-1015">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="325f4-1016">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="325f4-1016">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="325f4-1017">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1017">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1018">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1018">Appservice</span></span>

* <span data-ttu-id="325f4-1019">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="325f4-1019">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="325f4-1020">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1020">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="325f4-1021">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="325f4-1021">Eventhubs</span></span>

* <span data-ttu-id="325f4-1022">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1022">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-1023">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-1023">Extension</span></span>

* <span data-ttu-id="325f4-1024">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="325f4-1024">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-1025">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-1025">Interactive</span></span>

* <span data-ttu-id="325f4-1026">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="325f4-1026">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="325f4-1027">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="325f4-1027">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="325f4-1028">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="325f4-1028">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="325f4-1029">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="325f4-1029">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1030">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1030">Monitor</span></span>

* <span data-ttu-id="325f4-1031">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="325f4-1031">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="325f4-1032">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="325f4-1032">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="325f4-1033">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="325f4-1033">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="325f4-1034">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="325f4-1034">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1035">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1035">Network</span></span>

* <span data-ttu-id="325f4-1036">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1036">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="325f4-1037">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="325f4-1037">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="325f4-1038">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="325f4-1038">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="325f4-1039">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="325f4-1039">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1040">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1040">Profile</span></span>

* <span data-ttu-id="325f4-1041">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="325f4-1041">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="325f4-1042">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="325f4-1042">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-1043">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-1043">RDBMS</span></span>

* <span data-ttu-id="325f4-1044">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="325f4-1044">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="325f4-1045">Service Bus</span><span class="sxs-lookup"><span data-stu-id="325f4-1045">Service Bus</span></span>

* <span data-ttu-id="325f4-1046">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1046">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1047">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1047">Storage</span></span>

* <span data-ttu-id="325f4-1048">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="325f4-1048">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="325f4-1049">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="325f4-1049">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1050">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1050">VM</span></span>

* <span data-ttu-id="325f4-1051">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="325f4-1051">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="325f4-1052">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="325f4-1052">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="325f4-1053">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="325f4-1053">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="325f4-1054">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="325f4-1054">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="325f4-1055">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-1055">February 27, 2018</span></span>

<span data-ttu-id="325f4-1056">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="325f4-1056">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1057">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1057">Core</span></span>

* <span data-ttu-id="325f4-1058">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="325f4-1058">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="325f4-1059">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="325f4-1059">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="325f4-1060">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="325f4-1060">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1061">ACS</span></span>

* <span data-ttu-id="325f4-1062">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1062">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="325f4-1063">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="325f4-1063">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="325f4-1064">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="325f4-1064">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="325f4-1065">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="325f4-1065">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1066">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1066">Appservice</span></span>

* <span data-ttu-id="325f4-1067">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="325f4-1067">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="325f4-1068">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="325f4-1068">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="325f4-1069">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-1069">Cognitive Services</span></span>

* <span data-ttu-id="325f4-1070">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-1070">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="325f4-1071">Consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-1071">Consumption</span></span>

* <span data-ttu-id="325f4-1072">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="325f4-1072">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="325f4-1073">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="325f4-1073">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1074">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1074">Container</span></span>

* <span data-ttu-id="325f4-1075">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="325f4-1075">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1076">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1076">Network</span></span>

* <span data-ttu-id="325f4-1077">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="325f4-1077">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1078">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1078">Resource</span></span>

* <span data-ttu-id="325f4-1079">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="325f4-1079">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1080">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1080">Role</span></span>

* <span data-ttu-id="325f4-1081">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="325f4-1081">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1082">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1082">SQL</span></span>

* <span data-ttu-id="325f4-1083">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="325f4-1083">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1084">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1084">Storage</span></span>

* <span data-ttu-id="325f4-1085">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1085">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1086">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1086">VM</span></span>

* <span data-ttu-id="325f4-1087">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="325f4-1087">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="325f4-1088">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-1088">February 13, 2018</span></span>

<span data-ttu-id="325f4-1089">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="325f4-1089">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1090">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1090">Core</span></span>

* <span data-ttu-id="325f4-1091">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="325f4-1091">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1092">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1092">ACS</span></span>

* <span data-ttu-id="325f4-1093">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="325f4-1093">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="325f4-1094">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1094">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="325f4-1095">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="325f4-1095">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="325f4-1096">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-1096">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="325f4-1097">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="325f4-1097">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="325f4-1098">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="325f4-1098">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="325f4-1099">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="325f4-1099">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="325f4-1100">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="325f4-1100">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1101">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1101">Appservice</span></span>

* <span data-ttu-id="325f4-1102">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="325f4-1102">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="325f4-1103">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="325f4-1103">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="325f4-1104">CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-1104">CDN</span></span>

* <span data-ttu-id="325f4-1105">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1105">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1106">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1106">Container</span></span>

* <span data-ttu-id="325f4-1107">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="325f4-1107">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="325f4-1108">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1108">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="325f4-1109">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="325f4-1109">CosmosDB</span></span>

* <span data-ttu-id="325f4-1110">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="325f4-1110">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-1111">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-1111">Extension</span></span>

* <span data-ttu-id="325f4-1112">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1112">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="325f4-1113">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1113">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="325f4-1114">Commentaires</span><span class="sxs-lookup"><span data-stu-id="325f4-1114">Feedback</span></span>

* <span data-ttu-id="325f4-1115">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="325f4-1115">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-1116">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-1116">Interactive</span></span>

* <span data-ttu-id="325f4-1117">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="325f4-1117">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="325f4-1118">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="325f4-1118">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-1119">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1119">IoT</span></span>

* <span data-ttu-id="325f4-1120">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="325f4-1120">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="325f4-1121">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="325f4-1121">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="325f4-1122">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1122">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="325f4-1123">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="325f4-1123">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1124">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1124">Monitor</span></span>

* <span data-ttu-id="325f4-1125">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1125">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1126">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1126">Network</span></span>

* <span data-ttu-id="325f4-1127">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="325f4-1127">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="325f4-1128">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1128">Profile</span></span>

* <span data-ttu-id="325f4-1129">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="325f4-1129">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1130">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1130">Resource</span></span>

* <span data-ttu-id="325f4-1131">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1131">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1132">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1132">Role</span></span>

* <span data-ttu-id="325f4-1133">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1133">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1134">SQL</span></span>

* <span data-ttu-id="325f4-1135">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="325f4-1135">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="325f4-1136">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="325f4-1136">Added `sql db rename`</span></span>
* <span data-ttu-id="325f4-1137">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="325f4-1137">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1138">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1138">Storage</span></span>

* <span data-ttu-id="325f4-1139">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="325f4-1139">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1140">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1140">VM</span></span>

* <span data-ttu-id="325f4-1141">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="325f4-1141">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="325f4-1142">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="325f4-1142">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="325f4-1143">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="325f4-1143">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="325f4-1144">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-1144">January 31, 2018</span></span>

<span data-ttu-id="325f4-1145">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="325f4-1145">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1146">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1146">Core</span></span>

* <span data-ttu-id="325f4-1147">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="325f4-1147">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="325f4-1148">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-1148">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="325f4-1149">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="325f4-1149">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="325f4-1150">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="325f4-1150">Use `--verbose` to see</span></span>
* <span data-ttu-id="325f4-1151">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="325f4-1151">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1152">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1152">ACS</span></span>

* <span data-ttu-id="325f4-1153">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="325f4-1153">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="325f4-1154">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="325f4-1154">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1155">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1155">Appservice</span></span>

* <span data-ttu-id="325f4-1156">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="325f4-1156">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="325f4-1157">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="325f4-1157">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="325f4-1158">CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-1158">CDN</span></span>

* <span data-ttu-id="325f4-1159">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1159">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="325f4-1160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="325f4-1160">CosmosDB</span></span>

* <span data-ttu-id="325f4-1161">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="325f4-1161">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-1162">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-1162">Interactive</span></span>

* <span data-ttu-id="325f4-1163">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="325f4-1163">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1164">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1164">Network</span></span>

* <span data-ttu-id="325f4-1165">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1165">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="325f4-1166">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1166">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="325f4-1167">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1167">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="325f4-1168">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1168">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="325f4-1169">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="325f4-1169">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="325f4-1170">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="325f4-1170">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="325f4-1171">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="325f4-1171">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="325f4-1172">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="325f4-1172">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="325f4-1173">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="325f4-1173">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="325f4-1174">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="325f4-1174">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1175">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1175">Profile</span></span>

* <span data-ttu-id="325f4-1176">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="325f4-1176">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1177">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1177">Resource</span></span>

* <span data-ttu-id="325f4-1178">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="325f4-1178">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1179">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1179">Storage</span></span>

* <span data-ttu-id="325f4-1180">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="325f4-1180">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="325f4-1181">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="325f4-1181">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="325f4-1182">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-1182">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="325f4-1183">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1183">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="325f4-1184">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="325f4-1184">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1185">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1185">VM</span></span>

* <span data-ttu-id="325f4-1186">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="325f4-1186">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="325f4-1187">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="325f4-1187">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="325f4-1188">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="325f4-1188">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="325f4-1189">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1189">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="325f4-1190">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="325f4-1190">January 17, 2018</span></span>

<span data-ttu-id="325f4-1191">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="325f4-1191">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1192">ACR</span></span>

* <span data-ttu-id="325f4-1193">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-1193">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="325f4-1194">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="325f4-1194">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1195">ACS</span></span>

* <span data-ttu-id="325f4-1196">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="325f4-1196">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="325f4-1197">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="325f4-1197">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1198">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1198">Appservice</span></span>

* <span data-ttu-id="325f4-1199">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="325f4-1199">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="325f4-1200">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="325f4-1200">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="325f4-1201">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="325f4-1201">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="325f4-1202">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="325f4-1202">Backup</span></span>

* <span data-ttu-id="325f4-1203">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="325f4-1203">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="325f4-1204">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="325f4-1204">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="325f4-1205">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="325f4-1205">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="325f4-1206">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="325f4-1206">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="325f4-1207">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1207">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-1208">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1208">Batch</span></span>

* <span data-ttu-id="325f4-1209">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="325f4-1209">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="325f4-1210">Cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-1210">Cloud</span></span>

* <span data-ttu-id="325f4-1211">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-1211">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="325f4-1212">Consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-1212">Consumption</span></span>

* <span data-ttu-id="325f4-1213">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="325f4-1213">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="325f4-1214">Event Grid</span><span class="sxs-lookup"><span data-stu-id="325f4-1214">Event Grid</span></span>

* <span data-ttu-id="325f4-1215">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="325f4-1215">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="325f4-1216">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="325f4-1216">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="325f4-1217">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="325f4-1217">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="325f4-1218">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="325f4-1218">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="325f4-1219">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1219">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="325f4-1220">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1220">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="325f4-1221">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="325f4-1221">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="325f4-1222">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="325f4-1222">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-1223">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-1223">Interactive</span></span>

* <span data-ttu-id="325f4-1224">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="325f4-1224">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="325f4-1225">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="325f4-1225">Fixed errors on startup</span></span>
* <span data-ttu-id="325f4-1226">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="325f4-1226">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-1227">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1227">IoT</span></span>

* <span data-ttu-id="325f4-1228">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="325f4-1228">Added support for device provisioning service</span></span>
* <span data-ttu-id="325f4-1229">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-1229">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="325f4-1230">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1230">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1231">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1231">Monitor</span></span>

* <span data-ttu-id="325f4-1232">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="325f4-1232">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="325f4-1233">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1233">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="325f4-1234">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="325f4-1234">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1235">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1235">Network</span></span>

* <span data-ttu-id="325f4-1236">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1236">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="325f4-1237">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1237">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1238">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1238">Profile</span></span>

* <span data-ttu-id="325f4-1239">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="325f4-1239">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1240">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1240">Role</span></span>

* <span data-ttu-id="325f4-1241">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="325f4-1241">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="325f4-1242">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="325f4-1242">Service Fabric</span></span>

* <span data-ttu-id="325f4-1243">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="325f4-1243">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="325f4-1244">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-1244">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1245">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1245">VM</span></span>

* <span data-ttu-id="325f4-1246">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="325f4-1246">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="325f4-1247">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="325f4-1247">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="325f4-1248">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="325f4-1248">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="325f4-1249">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="325f4-1249">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="325f4-1250">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="325f4-1250">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="325f4-1251">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1251">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="325f4-1252">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1252">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="325f4-1253">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="325f4-1253">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="325f4-1254">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1254">December 19, 2017</span></span>

<span data-ttu-id="325f4-1255">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="325f4-1255">Version 2.0.23</span></span>

* <span data-ttu-id="325f4-1256">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="325f4-1256">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1257">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1257">Container</span></span>

* <span data-ttu-id="325f4-1258">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1258">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1259">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1259">Network</span></span>

* <span data-ttu-id="325f4-1260">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1260">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="325f4-1261">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1261">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1262">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1262">Storage</span></span>

* <span data-ttu-id="325f4-1263">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="325f4-1263">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1264">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1264">VM</span></span>

* <span data-ttu-id="325f4-1265">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="325f4-1265">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="325f4-1266">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1266">December 5, 2017</span></span>

<span data-ttu-id="325f4-1267">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="325f4-1267">Version 2.0.22</span></span>

* <span data-ttu-id="325f4-1268">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="325f4-1268">Removed `az component` commands.</span></span> <span data-ttu-id="325f4-1269">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="325f4-1269">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1270">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1270">Core</span></span>
* <span data-ttu-id="325f4-1271">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="325f4-1271">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="325f4-1272">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="325f4-1272">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1273">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1273">ACS</span></span>

* <span data-ttu-id="325f4-1274">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="325f4-1274">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="325f4-1275">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1275">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="325f4-1276">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="325f4-1276">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="325f4-1277">Advisor</span><span class="sxs-lookup"><span data-stu-id="325f4-1277">Advisor</span></span>

* <span data-ttu-id="325f4-1278">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1278">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1279">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1279">Appservice</span></span>

* <span data-ttu-id="325f4-1280">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="325f4-1280">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="325f4-1281">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="325f4-1281">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="325f4-1282">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="325f4-1282">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="325f4-1283">Consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-1283">Consumption</span></span>

* <span data-ttu-id="325f4-1284">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="325f4-1284">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1285">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1285">Container</span></span>

* <span data-ttu-id="325f4-1286">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1286">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1287">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1287">Monitor</span></span>

* <span data-ttu-id="325f4-1288">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="325f4-1288">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1289">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1289">Resource</span></span>

* <span data-ttu-id="325f4-1290">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1290">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1291">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1291">Role</span></span>

* <span data-ttu-id="325f4-1292">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="325f4-1292">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="325f4-1293">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="325f4-1293">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="325f4-1294">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="325f4-1294">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1295">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1295">SQL</span></span>

* <span data-ttu-id="325f4-1296">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="325f4-1296">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="325f4-1297">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1297">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1298">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1298">VM</span></span>

* <span data-ttu-id="325f4-1299">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="325f4-1299">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="325f4-1300">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1300">November 14, 2017</span></span>

<span data-ttu-id="325f4-1301">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="325f4-1301">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-1302">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1302">ACR</span></span>

* <span data-ttu-id="325f4-1303">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="325f4-1303">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="325f4-1304">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1304">ACS</span></span>

* <span data-ttu-id="325f4-1305">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="325f4-1305">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="325f4-1306">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1306">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="325f4-1307">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="325f4-1307">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="325f4-1308">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-1308">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="325f4-1309">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="325f4-1309">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1310">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1310">Appservice</span></span>

* <span data-ttu-id="325f4-1311">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="325f4-1311">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="325f4-1312">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="325f4-1312">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="325f4-1313">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="325f4-1313">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="325f4-1314">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="325f4-1314">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="325f4-1315">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="325f4-1315">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="325f4-1316">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="325f4-1316">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-1317">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1317">Batch</span></span>

* <span data-ttu-id="325f4-1318">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="325f4-1318">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="325f4-1319">Batchai</span><span class="sxs-lookup"><span data-stu-id="325f4-1319">Batchai</span></span>

* <span data-ttu-id="325f4-1320">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1320">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="325f4-1321">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1321">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="325f4-1322">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="325f4-1322">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="325f4-1323">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1323">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="325f4-1324">Cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-1324">Cloud</span></span>

* <span data-ttu-id="325f4-1325">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="325f4-1325">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1326">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1326">Container</span></span>

* <span data-ttu-id="325f4-1327">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="325f4-1327">Added support to open multiple ports</span></span>
* <span data-ttu-id="325f4-1328">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="325f4-1328">Added container group restart policy</span></span>
* <span data-ttu-id="325f4-1329">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="325f4-1329">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="325f4-1330">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="325f4-1330">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="325f4-1331">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="325f4-1331">Data Lake Analytics</span></span>

* <span data-ttu-id="325f4-1332">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="325f4-1332">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="325f4-1333">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1333">Data Lake Store</span></span>

* <span data-ttu-id="325f4-1334">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="325f4-1334">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-1335">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-1335">Extension</span></span>

* <span data-ttu-id="325f4-1336">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="325f4-1336">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="325f4-1337">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="325f4-1337">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-1338">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1338">IoT</span></span>

* <span data-ttu-id="325f4-1339">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="325f4-1339">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1340">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1340">Monitor</span></span>

* <span data-ttu-id="325f4-1341">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="325f4-1341">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1342">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1342">Network</span></span>

* <span data-ttu-id="325f4-1343">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="325f4-1343">Added support for CAA DNS records</span></span>
* <span data-ttu-id="325f4-1344">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1344">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="325f4-1345">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="325f4-1345">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="325f4-1346">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="325f4-1346">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="325f4-1347">Réservations</span><span class="sxs-lookup"><span data-stu-id="325f4-1347">Reservations</span></span>

* <span data-ttu-id="325f4-1348">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1348">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1349">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1349">Resource</span></span>

* <span data-ttu-id="325f4-1350">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="325f4-1350">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1351">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1351">SQL</span></span>

* <span data-ttu-id="325f4-1352">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1352">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1353">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1353">Storage</span></span>

* <span data-ttu-id="325f4-1354">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1354">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="325f4-1355">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="325f4-1355">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="325f4-1356">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="325f4-1356">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="325f4-1357">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="325f4-1357">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="325f4-1358">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1358">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="325f4-1359">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="325f4-1359">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="325f4-1360">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1360">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1361">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1361">VM</span></span>

* <span data-ttu-id="325f4-1362">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="325f4-1362">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="325f4-1363">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="325f4-1363">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="325f4-1364">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="325f4-1364">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="325f4-1365">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="325f4-1365">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="325f4-1366">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="325f4-1366">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="325f4-1367">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1367">October 24, 2017</span></span>

<span data-ttu-id="325f4-1368">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="325f4-1368">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1369">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1369">Core</span></span>

* <span data-ttu-id="325f4-1370">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="325f4-1370">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-1371">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1371">ACR</span></span>

* <span data-ttu-id="325f4-1372">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="325f4-1372">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="325f4-1373">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="325f4-1373">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="325f4-1374">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="325f4-1374">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1375">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1375">ACS</span></span>

* <span data-ttu-id="325f4-1376">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="325f4-1376">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="325f4-1377">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="325f4-1377">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1378">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1378">Appservice</span></span>

* <span data-ttu-id="325f4-1379">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="325f4-1379">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="325f4-1380">Composant</span><span class="sxs-lookup"><span data-stu-id="325f4-1380">Component</span></span>

* <span data-ttu-id="325f4-1381">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="325f4-1381">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1382">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1382">Monitor</span></span>

* <span data-ttu-id="325f4-1383">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="325f4-1383">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1384">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1384">Resource</span></span>

* <span data-ttu-id="325f4-1385">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="325f4-1385">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="325f4-1386">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="325f4-1386">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1387">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1387">VM</span></span>

* <span data-ttu-id="325f4-1388">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1388">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="325f4-1389">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1389">October 9, 2017</span></span>

<span data-ttu-id="325f4-1390">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="325f4-1390">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1391">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1391">Core</span></span>

* <span data-ttu-id="325f4-1392">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="325f4-1392">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1393">Appservice</span></span>

* <span data-ttu-id="325f4-1394">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1394">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-1395">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1395">Batch</span></span>

* <span data-ttu-id="325f4-1396">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="325f4-1396">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="325f4-1397">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="325f4-1397">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="325f4-1398">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1398">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="325f4-1399">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="325f4-1399">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="325f4-1400">Batchai</span><span class="sxs-lookup"><span data-stu-id="325f4-1400">Batchai</span></span>

* <span data-ttu-id="325f4-1401">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="325f4-1401">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-1402">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-1402">Keyvault</span></span>

* <span data-ttu-id="325f4-1403">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="325f4-1403">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="325f4-1404">(#4448)</span><span class="sxs-lookup"><span data-stu-id="325f4-1404">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="325f4-1405">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1405">Network</span></span>

* <span data-ttu-id="325f4-1406">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="325f4-1406">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="325f4-1407">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="325f4-1407">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1408">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1408">Resource</span></span>

* <span data-ttu-id="325f4-1409">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="325f4-1409">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="325f4-1410">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-1410">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="325f4-1411">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="325f4-1411">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="325f4-1412">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="325f4-1412">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1413">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1413">Sql</span></span>

* <span data-ttu-id="325f4-1414">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="325f4-1414">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="325f4-1415">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="325f4-1415">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="325f4-1416">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="325f4-1416">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1417">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1417">Storage</span></span>

* <span data-ttu-id="325f4-1418">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="325f4-1418">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1419">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1419">Vm</span></span>

* <span data-ttu-id="325f4-1420">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="325f4-1420">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="325f4-1421">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1421">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="325f4-1422">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="325f4-1422">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="325f4-1423">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1423">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="325f4-1424">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1424">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="325f4-1425">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1425">September 22, 2017</span></span>

<span data-ttu-id="325f4-1426">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="325f4-1426">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1427">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1427">Resource</span></span>

* <span data-ttu-id="325f4-1428">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="325f4-1428">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="325f4-1429">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="325f4-1429">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="325f4-1430">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1430">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="325f4-1431">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="325f4-1431">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1432">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1432">Network</span></span>

* <span data-ttu-id="325f4-1433">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="325f4-1433">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="325f4-1434">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="325f4-1434">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="325f4-1435">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="325f4-1435">Added `asg` application security group commands</span></span>
* <span data-ttu-id="325f4-1436">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1436">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="325f4-1437">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1437">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="325f4-1438">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1438">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="325f4-1439">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1439">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1440">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1440">Storage</span></span>

* <span data-ttu-id="325f4-1441">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="325f4-1441">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="325f4-1442">Événement</span><span class="sxs-lookup"><span data-stu-id="325f4-1442">Eventgrid</span></span>

* <span data-ttu-id="325f4-1443">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="325f4-1443">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1444">SQL</span></span>

* <span data-ttu-id="325f4-1445">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="325f4-1445">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="325f4-1446">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="325f4-1446">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="325f4-1447">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1447">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-1448">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-1448">Keyvault</span></span>

* <span data-ttu-id="325f4-1449">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="325f4-1449">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1450">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1450">VM</span></span>

* <span data-ttu-id="325f4-1451">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1451">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="325f4-1452">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="325f4-1452">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="325f4-1453">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1453">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="325f4-1454">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="325f4-1454">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="325f4-1455">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="325f4-1455">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="325f4-1456">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="325f4-1456">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1457">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1457">ACS</span></span>

* <span data-ttu-id="325f4-1458">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="325f4-1458">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1459">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1459">Appservice</span></span>

* <span data-ttu-id="325f4-1460">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1460">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="325f4-1461">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="325f4-1461">Backup</span></span>

* <span data-ttu-id="325f4-1462">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="325f4-1462">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="325f4-1463">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1463">September 11, 2017</span></span>

<span data-ttu-id="325f4-1464">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="325f4-1464">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="325f4-1465">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1465">Core</span></span>

* <span data-ttu-id="325f4-1466">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="325f4-1466">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="325f4-1467">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="325f4-1467">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1468">Acs</span><span class="sxs-lookup"><span data-stu-id="325f4-1468">Acs</span></span>

* <span data-ttu-id="325f4-1469">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="325f4-1469">Added `acs list-locations` command</span></span>
* <span data-ttu-id="325f4-1470">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="325f4-1470">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1471">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1471">Appservice</span></span>

* <span data-ttu-id="325f4-1472">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="325f4-1472">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="325f4-1473">CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-1473">CDN</span></span>

* <span data-ttu-id="325f4-1474">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1474">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="325f4-1475">Extension</span><span class="sxs-lookup"><span data-stu-id="325f4-1475">Extension</span></span>

* <span data-ttu-id="325f4-1476">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1476">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-1477">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-1477">Keyvault</span></span>

* <span data-ttu-id="325f4-1478">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="325f4-1478">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1479">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1479">Network</span></span>

* <span data-ttu-id="325f4-1480">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="325f4-1480">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="325f4-1481">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1481">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="325f4-1482">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1482">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="325f4-1483">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1483">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="325f4-1484">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1484">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1485">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1485">Resource</span></span>

* <span data-ttu-id="325f4-1486">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1486">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="325f4-1487">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1487">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="325f4-1488">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="325f4-1488">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="325f4-1489">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="325f4-1489">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1490">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1490">SQL</span></span>

* <span data-ttu-id="325f4-1491">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="325f4-1491">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1492">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1492">VM</span></span>

* <span data-ttu-id="325f4-1493">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="325f4-1493">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="325f4-1494">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="325f4-1494">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="325f4-1495">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1495">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="325f4-1496">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="325f4-1496">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="325f4-1497">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="325f4-1497">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="325f4-1498">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1498">August 31, 2017</span></span>

<span data-ttu-id="325f4-1499">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="325f4-1499">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-1500">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-1500">Keyvault</span></span>

* <span data-ttu-id="325f4-1501">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="325f4-1501">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="325f4-1502">Sf</span><span class="sxs-lookup"><span data-stu-id="325f4-1502">Sf</span></span>

* <span data-ttu-id="325f4-1503">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="325f4-1503">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1504">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1504">Storage</span></span>

* <span data-ttu-id="325f4-1505">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="325f4-1505">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="325f4-1506">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="325f4-1506">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="325f4-1507">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1507">August 28, 2017</span></span>

<span data-ttu-id="325f4-1508">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="325f4-1508">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="325f4-1509">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="325f4-1509">CLI</span></span>

* <span data-ttu-id="325f4-1510">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="325f4-1510">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1511">ACS</span></span>

* <span data-ttu-id="325f4-1512">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="325f4-1512">Corrected preview regions</span></span>
* <span data-ttu-id="325f4-1513">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-1513">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="325f4-1514">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1514">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1515">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1515">Appservice</span></span>

* <span data-ttu-id="325f4-1516">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1516">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="325f4-1517">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-1517">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="325f4-1518">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1518">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="325f4-1519">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="325f4-1519">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="325f4-1520">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-1520">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-1521">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1521">IoT</span></span>

* <span data-ttu-id="325f4-1522">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="325f4-1522">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1523">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1523">Network</span></span>

* <span data-ttu-id="325f4-1524">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="325f4-1524">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="325f4-1525">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1525">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="325f4-1526">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="325f4-1526">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="325f4-1527">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1527">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="325f4-1528">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1528">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1529">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1529">Profile</span></span>

* <span data-ttu-id="325f4-1530">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1530">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="325f4-1531">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="325f4-1531">Service Fabric</span></span>

* <span data-ttu-id="325f4-1532">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="325f4-1532">Preview release</span></span>
* <span data-ttu-id="325f4-1533">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="325f4-1533">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="325f4-1534">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="325f4-1534">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="325f4-1535">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="325f4-1535">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1536">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1536">Storage</span></span>

* <span data-ttu-id="325f4-1537">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="325f4-1537">Enabled setting blob tier</span></span>
* <span data-ttu-id="325f4-1538">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="325f4-1538">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="325f4-1539">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="325f4-1539">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="325f4-1540">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="325f4-1540">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="325f4-1541">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1541">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="325f4-1542">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="325f4-1542">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1543">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1543">VM</span></span>

* <span data-ttu-id="325f4-1544">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="325f4-1544">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="325f4-1545">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="325f4-1545">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="325f4-1546">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1546">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="325f4-1547">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="325f4-1547">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="325f4-1548">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="325f4-1548">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="325f4-1549">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1549">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="325f4-1550">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1550">August 15, 2017</span></span>

<span data-ttu-id="325f4-1551">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="325f4-1551">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1552">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1552">ACS</span></span>

* <span data-ttu-id="325f4-1553">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="325f4-1553">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1554">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1554">Appservice</span></span>

* <span data-ttu-id="325f4-1555">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="325f4-1555">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="325f4-1556">Event Grid</span><span class="sxs-lookup"><span data-stu-id="325f4-1556">Event Grid</span></span>

* <span data-ttu-id="325f4-1557">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="325f4-1557">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="325f4-1558">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1558">August 11, 2017</span></span>

<span data-ttu-id="325f4-1559">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="325f4-1559">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1560">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1560">ACS</span></span>

* <span data-ttu-id="325f4-1561">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="325f4-1561">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-1562">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1562">Batch</span></span>

* <span data-ttu-id="325f4-1563">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="325f4-1563">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="325f4-1564">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="325f4-1564">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="325f4-1565">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="325f4-1565">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="325f4-1566">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="325f4-1566">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="325f4-1567">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="325f4-1567">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="325f4-1568">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="325f4-1568">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="325f4-1569">Composant</span><span class="sxs-lookup"><span data-stu-id="325f4-1569">Component</span></span>

* <span data-ttu-id="325f4-1570">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="325f4-1570">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="325f4-1571">Conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1571">Container</span></span>

* <span data-ttu-id="325f4-1572">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="325f4-1572">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="325f4-1573">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1573">Data Lake Store</span></span>

* <span data-ttu-id="325f4-1574">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="325f4-1574">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="325f4-1575">Event Grid</span><span class="sxs-lookup"><span data-stu-id="325f4-1575">Event Grid</span></span>

* <span data-ttu-id="325f4-1576">Version initiale</span><span class="sxs-lookup"><span data-stu-id="325f4-1576">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1577">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1577">Network</span></span>

* <span data-ttu-id="325f4-1578">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="325f4-1578">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="325f4-1579">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="325f4-1579">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="325f4-1580">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="325f4-1580">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="325f4-1581">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="325f4-1581">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1582">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1582">Profile</span></span>

* <span data-ttu-id="325f4-1583">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="325f4-1583">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1584">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1584">Storage</span></span>

* <span data-ttu-id="325f4-1585">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="325f4-1585">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1586">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1586">VM</span></span>

* <span data-ttu-id="325f4-1587">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="325f4-1587">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="325f4-1588">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="325f4-1588">Exposed `list-skus` command</span></span>
* <span data-ttu-id="325f4-1589">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1589">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="325f4-1590">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="325f4-1590">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="325f4-1591">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="325f4-1591">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="325f4-1592">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1592">July 28, 2017</span></span>

<span data-ttu-id="325f4-1593">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="325f4-1593">Version 2.0.12</span></span>

* <span data-ttu-id="325f4-1594">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="325f4-1594">Added container commands</span></span>
* <span data-ttu-id="325f4-1595">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="325f4-1595">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="325f4-1596">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1596">Core</span></span>

* <span data-ttu-id="325f4-1597">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="325f4-1597">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="325f4-1598">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="325f4-1598">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="325f4-1599">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="325f4-1599">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="325f4-1600">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="325f4-1600">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="325f4-1601">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="325f4-1601">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="325f4-1602">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="325f4-1602">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="325f4-1603">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="325f4-1603">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="325f4-1604">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="325f4-1604">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="325f4-1605">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="325f4-1605">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="325f4-1606">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="325f4-1606">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="325f4-1607">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="325f4-1607">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="325f4-1608">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="325f4-1608">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="325f4-1609">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="325f4-1609">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="325f4-1610">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="325f4-1610">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="325f4-1611">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="325f4-1611">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="325f4-1612">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="325f4-1612">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="325f4-1613">ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1613">ACR</span></span>

* <span data-ttu-id="325f4-1614">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="325f4-1614">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="325f4-1615">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="325f4-1615">Support SKU update for managed registries</span></span>
* <span data-ttu-id="325f4-1616">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="325f4-1616">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="325f4-1617">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="325f4-1617">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="325f4-1618">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="325f4-1618">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="325f4-1619">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="325f4-1619">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1620">ACS</span></span>

* <span data-ttu-id="325f4-1621">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="325f4-1621">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1622">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1622">Appservice</span></span>

* <span data-ttu-id="325f4-1623">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="325f4-1623">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="325f4-1624">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="325f4-1624">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="325f4-1625">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="325f4-1625">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="325f4-1626">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="325f4-1626">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="325f4-1627">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="325f4-1627">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="325f4-1628">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="325f4-1628">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="325f4-1629">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="325f4-1629">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="325f4-1630">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="325f4-1630">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="325f4-1631">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="325f4-1631">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="325f4-1632">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="325f4-1632">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="325f4-1633">Batch</span><span class="sxs-lookup"><span data-stu-id="325f4-1633">Batch</span></span>

* <span data-ttu-id="325f4-1634">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="325f4-1634">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="325f4-1635">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="325f4-1635">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="325f4-1636">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="325f4-1636">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="325f4-1637">CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-1637">CDN</span></span>

* <span data-ttu-id="325f4-1638">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="325f4-1638">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="325f4-1639">Cloud</span><span class="sxs-lookup"><span data-stu-id="325f4-1639">Cloud</span></span>

* <span data-ttu-id="325f4-1640">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="325f4-1640">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="325f4-1641">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="325f4-1641">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="325f4-1642">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="325f4-1642">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="325f4-1643">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="325f4-1643">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="325f4-1644">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="325f4-1644">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="325f4-1645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="325f4-1645">CosmosDB</span></span>

* <span data-ttu-id="325f4-1646">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="325f4-1646">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="325f4-1647">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="325f4-1647">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="325f4-1648">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="325f4-1648">Data Lake Analytics</span></span>

* <span data-ttu-id="325f4-1649">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="325f4-1649">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="325f4-1650">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1650">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="325f4-1651">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="325f4-1651">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="325f4-1652">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1652">Data Lake Store</span></span>

* <span data-ttu-id="325f4-1653">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1653">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="325f4-1654">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="325f4-1654">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="325f4-1655">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="325f4-1655">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="325f4-1656">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1656">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="325f4-1657">Interactive</span><span class="sxs-lookup"><span data-stu-id="325f4-1657">Interactive</span></span>

* <span data-ttu-id="325f4-1658">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="325f4-1658">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="325f4-1659">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="325f4-1659">Increased test coverage</span></span>
* <span data-ttu-id="325f4-1660">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="325f4-1660">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="325f4-1661">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="325f4-1661">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="325f4-1662">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="325f4-1662">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="325f4-1663">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="325f4-1663">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="325f4-1664">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="325f4-1664">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="325f4-1665">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="325f4-1665">Added `--progress` flag</span></span>
* <span data-ttu-id="325f4-1666">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="325f4-1666">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="325f4-1667">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="325f4-1667">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="325f4-1668">IoT</span><span class="sxs-lookup"><span data-stu-id="325f4-1668">IoT</span></span>

* <span data-ttu-id="325f4-1669">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="325f4-1669">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="325f4-1670">(#3934)</span><span class="sxs-lookup"><span data-stu-id="325f4-1670">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="325f4-1671">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="325f4-1671">Key vault</span></span>

* <span data-ttu-id="325f4-1672">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="325f4-1672">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="325f4-1673">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="325f4-1673">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="325f4-1674">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="325f4-1674">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="325f4-1675">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="325f4-1675">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="325f4-1676">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="325f4-1676">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="325f4-1677">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="325f4-1677">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="325f4-1678">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="325f4-1678">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="325f4-1679">(#3307)</span><span class="sxs-lookup"><span data-stu-id="325f4-1679">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="325f4-1680">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1680">Lab</span></span>

* <span data-ttu-id="325f4-1681">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="325f4-1681">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="325f4-1682">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1682">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1683">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1683">Monitor</span></span>

* <span data-ttu-id="325f4-1684">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="325f4-1684">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="325f4-1685">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="325f4-1685">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="325f4-1686">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="325f4-1686">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="325f4-1687">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="325f4-1687">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="325f4-1688">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="325f4-1688">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="325f4-1689">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="325f4-1689">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="325f4-1690">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="325f4-1690">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="325f4-1691">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="325f4-1691">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="325f4-1692">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="325f4-1692">`location` no longer required</span></span>
  * <span data-ttu-id="325f4-1693">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="325f4-1693">Add name and ID support for target</span></span>
  * <span data-ttu-id="325f4-1694">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-1694">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="325f4-1695">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="325f4-1695">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="325f4-1696">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="325f4-1696">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="325f4-1697">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="325f4-1697">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="325f4-1698">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="325f4-1698">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="325f4-1699">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1699">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1700">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1700">Network</span></span>

* <span data-ttu-id="325f4-1701">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="325f4-1701">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="325f4-1702">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1702">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="325f4-1703">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="325f4-1703">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="325f4-1704">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="325f4-1704">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="325f4-1705">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1705">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="325f4-1706">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="325f4-1706">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="325f4-1707">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1707">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="325f4-1708">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="325f4-1708">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="325f4-1709">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="325f4-1709">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="325f4-1710">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="325f4-1710">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="325f4-1711">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1711">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="325f4-1712">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="325f4-1712">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="325f4-1713">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="325f4-1713">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="325f4-1714">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1714">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="325f4-1715">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1715">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="325f4-1716">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1716">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="325f4-1717">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="325f4-1717">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="325f4-1718">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="325f4-1718">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="325f4-1719">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1719">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="325f4-1720">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1720">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="325f4-1721">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1721">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="325f4-1722">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1722">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="325f4-1723">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="325f4-1723">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="325f4-1724">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="325f4-1724">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="325f4-1725">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="325f4-1725">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="325f4-1726">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="325f4-1726">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="325f4-1727">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="325f4-1727">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1728">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1728">Profile</span></span>

* <span data-ttu-id="325f4-1729">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="325f4-1729">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="325f4-1730">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="325f4-1730">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="325f4-1731">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="325f4-1731">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="325f4-1732">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="325f4-1732">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="325f4-1733">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="325f4-1733">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="325f4-1734">SGBDR</span><span class="sxs-lookup"><span data-stu-id="325f4-1734">RDBMS</span></span>

* <span data-ttu-id="325f4-1735">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="325f4-1735">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="325f4-1736">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="325f4-1736">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="325f4-1737">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="325f4-1737">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="325f4-1738">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="325f4-1738">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1739">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1739">Resource</span></span>

* <span data-ttu-id="325f4-1740">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1740">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="325f4-1741">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="325f4-1741">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="325f4-1742">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="325f4-1742">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="325f4-1743">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="325f4-1743">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="325f4-1744">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="325f4-1744">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="325f4-1745">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="325f4-1745">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="325f4-1746">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="325f4-1746">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="325f4-1747">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="325f4-1747">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1748">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1748">Role</span></span>

* <span data-ttu-id="325f4-1749">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="325f4-1749">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="325f4-1750">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="325f4-1750">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="325f4-1751">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="325f4-1751">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="325f4-1752">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="325f4-1752">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="325f4-1753">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="325f4-1753">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="325f4-1754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="325f4-1754">Service Fabric</span></span>
* <span data-ttu-id="325f4-1755">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="325f4-1755">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="325f4-1756">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="325f4-1756">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="325f4-1757">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="325f4-1757">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1758">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1758">SQL</span></span>

* <span data-ttu-id="325f4-1759">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="325f4-1759">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="325f4-1760">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="325f4-1760">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="325f4-1761">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="325f4-1761">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1762">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1762">Storage</span></span>

* <span data-ttu-id="325f4-1763">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="325f4-1763">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="325f4-1764">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="325f4-1764">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="325f4-1765">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="325f4-1765">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="325f4-1766">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="325f4-1766">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="325f4-1767">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="325f4-1767">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="325f4-1768">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="325f4-1768">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1769">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1769">VM</span></span>

* <span data-ttu-id="325f4-1770">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1770">Support configuring nsg</span></span>
* <span data-ttu-id="325f4-1771">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="325f4-1771">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="325f4-1772">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="325f4-1772">Support managed service identities</span></span>
* <span data-ttu-id="325f4-1773">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="325f4-1773">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="325f4-1774">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="325f4-1774">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="325f4-1775">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1775">May 10, 2017</span></span>

<span data-ttu-id="325f4-1776">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="325f4-1776">Version 2.0.6</span></span>

* <span data-ttu-id="325f4-1777">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="325f4-1777">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="325f4-1778">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="325f4-1778">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="325f4-1779">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1779">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="325f4-1780">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="325f4-1780">Include Cognitive Services module</span></span>
* <span data-ttu-id="325f4-1781">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="325f4-1781">Include Service Fabric module</span></span>
* <span data-ttu-id="325f4-1782">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="325f4-1782">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="325f4-1783">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="325f4-1783">Add support for CDN commands</span></span>
* <span data-ttu-id="325f4-1784">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="325f4-1784">Remove Container module</span></span>
* <span data-ttu-id="325f4-1785">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="325f4-1785">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="325f4-1786">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="325f4-1786">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="325f4-1787">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1787">Core</span></span>

* <span data-ttu-id="325f4-1788">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="325f4-1788">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="325f4-1789">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="325f4-1789">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="325f4-1790">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="325f4-1790">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="325f4-1791">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="325f4-1791">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="325f4-1792">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="325f4-1792">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="325f4-1793">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="325f4-1793">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="325f4-1794">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="325f4-1794">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="325f4-1795">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="325f4-1795">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="325f4-1796">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="325f4-1796">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="325f4-1797">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="325f4-1797">core: Improved performance</span></span>
* <span data-ttu-id="325f4-1798">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="325f4-1798">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="325f4-1799">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="325f4-1799">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1800">ACS</span></span>

* <span data-ttu-id="325f4-1801">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="325f4-1801">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="325f4-1802">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="325f4-1802">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="325f4-1803">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="325f4-1803">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="325f4-1804">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="325f4-1804">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1805">AppService</span></span>

* <span data-ttu-id="325f4-1806">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="325f4-1806">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="325f4-1807">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="325f4-1807">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="325f4-1808">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="325f4-1808">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="325f4-1809">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="325f4-1809">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="325f4-1810">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="325f4-1810">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="325f4-1811">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="325f4-1811">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="325f4-1812">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="325f4-1812">support slot swap with preview</span></span>
* <span data-ttu-id="325f4-1813">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="325f4-1813">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="325f4-1814">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="325f4-1814">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="325f4-1815">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="325f4-1815">CosmosDB</span></span>

* <span data-ttu-id="325f4-1816">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="325f4-1816">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="325f4-1817">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="325f4-1817">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="325f4-1818">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="325f4-1818">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="325f4-1819">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="325f4-1819">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="325f4-1820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="325f4-1820">Data Lake Analytics</span></span>

* <span data-ttu-id="325f4-1821">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="325f4-1821">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="325f4-1822">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="325f4-1822">Add support for new catalog item type: package.</span></span> <span data-ttu-id="325f4-1823">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="325f4-1823">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="325f4-1824">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="325f4-1824">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="325f4-1825">Table</span><span class="sxs-lookup"><span data-stu-id="325f4-1825">Table</span></span>
  * <span data-ttu-id="325f4-1826">Fonction table</span><span class="sxs-lookup"><span data-stu-id="325f4-1826">Table valued function</span></span>
  * <span data-ttu-id="325f4-1827">Affichage</span><span class="sxs-lookup"><span data-stu-id="325f4-1827">View</span></span>
  * <span data-ttu-id="325f4-1828">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="325f4-1828">Table Statistics.</span></span> <span data-ttu-id="325f4-1829">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="325f4-1829">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="325f4-1830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1830">Data Lake Store</span></span>

* <span data-ttu-id="325f4-1831">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="325f4-1831">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="325f4-1832">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="325f4-1832">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="325f4-1833">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="325f4-1833">missed help for access show.</span></span> <span data-ttu-id="325f4-1834">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="325f4-1834">adding it.</span></span> <span data-ttu-id="325f4-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="325f4-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="325f4-1836">Rechercher</span><span class="sxs-lookup"><span data-stu-id="325f4-1836">Find</span></span>

* <span data-ttu-id="325f4-1837">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="325f4-1837">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="325f4-1838">KeyVault</span><span class="sxs-lookup"><span data-stu-id="325f4-1838">KeyVault</span></span>

* <span data-ttu-id="325f4-1839">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="325f4-1839">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="325f4-1840">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="325f4-1840">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="325f4-1841">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="325f4-1841">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="325f4-1842">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="325f4-1842">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="325f4-1843">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="325f4-1843">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="325f4-1844">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1844">Lab</span></span>

* <span data-ttu-id="325f4-1845">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1845">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="325f4-1846">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1846">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="325f4-1847">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1847">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="325f4-1848">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1848">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="325f4-1849">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="325f4-1849">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="325f4-1850">Surveiller</span><span class="sxs-lookup"><span data-stu-id="325f4-1850">Monitor</span></span>

* <span data-ttu-id="325f4-1851">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="325f4-1851">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="325f4-1852">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="325f4-1852">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="325f4-1853">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1853">Network</span></span>

* <span data-ttu-id="325f4-1854">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="325f4-1854">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="325f4-1855">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1855">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="325f4-1856">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="325f4-1856">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="325f4-1857">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="325f4-1857">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="325f4-1858">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="325f4-1858">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="325f4-1859">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="325f4-1859">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="325f4-1860">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="325f4-1860">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="325f4-1861">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="325f4-1861">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="325f4-1862">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="325f4-1862">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="325f4-1863">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="325f4-1863">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="325f4-1864">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="325f4-1864">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="325f4-1865">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1865">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="325f4-1866">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-1866">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="325f4-1867">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="325f4-1867">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="325f4-1868">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="325f4-1868">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="325f4-1869">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="325f4-1869">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="325f4-1870">Profil</span><span class="sxs-lookup"><span data-stu-id="325f4-1870">Profile</span></span>

* <span data-ttu-id="325f4-1871">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="325f4-1871">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="325f4-1872">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="325f4-1872">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="325f4-1873">Redis</span><span class="sxs-lookup"><span data-stu-id="325f4-1873">Redis</span></span>

* <span data-ttu-id="325f4-1874">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="325f4-1874">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="325f4-1875">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="325f4-1875">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="325f4-1876">Ressource</span><span class="sxs-lookup"><span data-stu-id="325f4-1876">Resource</span></span>

* <span data-ttu-id="325f4-1877">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="325f4-1877">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="325f4-1878">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="325f4-1878">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="325f4-1879">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="325f4-1879">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="325f4-1880">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="325f4-1880">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="325f4-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="325f4-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="325f4-1882">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="325f4-1882">Add docs for az lock update.</span></span> <span data-ttu-id="325f4-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="325f4-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="325f4-1884">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="325f4-1884">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="325f4-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="325f4-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="325f4-1886">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="325f4-1886">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="325f4-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="325f4-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="325f4-1888">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="325f4-1888">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="325f4-1889">Rôle</span><span class="sxs-lookup"><span data-stu-id="325f4-1889">Role</span></span>

* <span data-ttu-id="325f4-1890">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="325f4-1890">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="325f4-1891">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="325f4-1891">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="325f4-1892">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="325f4-1892">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="325f4-1893">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="325f4-1893">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="325f4-1894">SQL</span><span class="sxs-lookup"><span data-stu-id="325f4-1894">SQL</span></span>

* <span data-ttu-id="325f4-1895">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="325f4-1895">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="325f4-1896">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="325f4-1896">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="325f4-1897">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1897">Storage</span></span>

* <span data-ttu-id="325f4-1898">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="325f4-1898">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="325f4-1899">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="325f4-1899">Add support for incremental blob copy</span></span>
* <span data-ttu-id="325f4-1900">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="325f4-1900">Add support for large block blob upload</span></span>
* <span data-ttu-id="325f4-1901">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="325f4-1901">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1902">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1902">VM</span></span>

* <span data-ttu-id="325f4-1903">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="325f4-1903">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="325f4-1904">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="325f4-1904">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="325f4-1905">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="325f4-1905">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="325f4-1906">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="325f4-1906">az vm/vmss disk</span></span>
  3. <span data-ttu-id="325f4-1907">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="325f4-1907">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="325f4-1908">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="325f4-1908">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="325f4-1909">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="325f4-1909">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="325f4-1910">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1910">April 3, 2017</span></span>

<span data-ttu-id="325f4-1911">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="325f4-1911">Version 2.0.2</span></span>

<span data-ttu-id="325f4-1912">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="325f4-1912">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="325f4-1913">Principal</span><span class="sxs-lookup"><span data-stu-id="325f4-1913">Core</span></span>

* <span data-ttu-id="325f4-1914">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1914">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="325f4-1915">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="325f4-1915">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="325f4-1916">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="325f4-1916">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="325f4-1917">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="325f4-1917">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="325f4-1918">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="325f4-1918">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="325f4-1919">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="325f4-1919">Add prompting for missing template parameters.</span></span> <span data-ttu-id="325f4-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="325f4-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="325f4-1921">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="325f4-1921">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="325f4-1922">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="325f4-1922">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="325f4-1923">ACS</span><span class="sxs-lookup"><span data-stu-id="325f4-1923">ACS</span></span>

* <span data-ttu-id="325f4-1924">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="325f4-1924">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="325f4-1925">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="325f4-1925">Add support for ssh key password prompting.</span></span> <span data-ttu-id="325f4-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="325f4-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="325f4-1927">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="325f4-1927">Add support for windows clusters.</span></span> <span data-ttu-id="325f4-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="325f4-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="325f4-1929">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="325f4-1929">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="325f4-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="325f4-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="325f4-1931">AppService</span><span class="sxs-lookup"><span data-stu-id="325f4-1931">AppService</span></span>

* <span data-ttu-id="325f4-1932">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="325f4-1932">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="325f4-1933">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="325f4-1933">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="325f4-1934">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="325f4-1934">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="325f4-1935">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="325f4-1935">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="325f4-1936">DataLake</span><span class="sxs-lookup"><span data-stu-id="325f4-1936">DataLake</span></span>

* <span data-ttu-id="325f4-1937">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="325f4-1937">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="325f4-1938">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="325f4-1938">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="325f4-1939">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="325f4-1939">DocuemntDB</span></span>

* <span data-ttu-id="325f4-1940">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="325f4-1940">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="325f4-1941">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="325f4-1941">VM</span></span>

* <span data-ttu-id="325f4-1942">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="325f4-1942">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="325f4-1943">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="325f4-1943">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="325f4-1944">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="325f4-1944">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="325f4-1945">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="325f4-1945">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="325f4-1946">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="325f4-1946">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="325f4-1947">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="325f4-1947">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="325f4-1948">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="325f4-1948">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="325f4-1949">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="325f4-1949">February 27, 2017</span></span>

<span data-ttu-id="325f4-1950">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="325f4-1950">Version 2.0.0</span></span>

<span data-ttu-id="325f4-1951">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="325f4-1951">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="325f4-1952">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="325f4-1952">Container Service (acs)</span></span>
- <span data-ttu-id="325f4-1953">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="325f4-1953">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="325f4-1954">Réseau</span><span class="sxs-lookup"><span data-stu-id="325f4-1954">Networking</span></span>
- <span data-ttu-id="325f4-1955">Stockage</span><span class="sxs-lookup"><span data-stu-id="325f4-1955">Storage</span></span>

<span data-ttu-id="325f4-1956">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="325f4-1956">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="325f4-1957">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="325f4-1957">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="325f4-1958">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="325f4-1958">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="325f4-1959">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="325f4-1959">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="325f4-1960">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="325f4-1960">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="325f4-1961">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="325f4-1961">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="325f4-1962">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="325f4-1962">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="325f4-1963">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="325f4-1963">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="325f4-1964">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="325f4-1964">Provide feedback from the command line with the `az feedback` command</span></span>

