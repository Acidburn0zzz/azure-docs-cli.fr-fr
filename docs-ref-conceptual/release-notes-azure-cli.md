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
ms.openlocfilehash: 36b57d52a5851275fd317240e5c2c95171a99e7e
ms.sourcegitcommit: 22b73d56602c1c4e647ed2c5af3d596a2f6a7ed5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/21/2018
ms.locfileid: "52267328"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="c5a65-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c5a65-103">Azure CLI release notes</span></span>
## <a name="november-20-2018"></a><span data-ttu-id="c5a65-104">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-104">November 20, 2018</span></span>

<span data-ttu-id="c5a65-105">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="c5a65-105">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="c5a65-106">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-106">Core</span></span>
* <span data-ttu-id="c5a65-107">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="c5a65-107">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-108">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-108">ACR</span></span>
* <span data-ttu-id="c5a65-109">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="c5a65-109">Added context token to task step</span></span>
* <span data-ttu-id="c5a65-110">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="c5a65-110">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="c5a65-111">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c5a65-111">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-112">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-112">Appservice</span></span>
* <span data-ttu-id="c5a65-113">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="c5a65-113">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="c5a65-114">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-114">Updated the default `node_version`.</span></span> <span data-ttu-id="c5a65-115">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="c5a65-115">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="c5a65-116">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="c5a65-116">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="c5a65-117">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="c5a65-117">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c5a65-118">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c5a65-118">IotCentral</span></span>
* <span data-ttu-id="c5a65-119">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="c5a65-119">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-120">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-120">KeyVault</span></span>
* <span data-ttu-id="c5a65-121">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="c5a65-121">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-122">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-122">Network</span></span>
* <span data-ttu-id="c5a65-123">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="c5a65-123">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="c5a65-124">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="c5a65-124">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="c5a65-125">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-125">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="c5a65-126">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="c5a65-126">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c5a65-127">Rdbms</span></span>
* <span data-ttu-id="c5a65-128">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="c5a65-128">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="c5a65-129">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="c5a65-129">Rbac</span></span>
* <span data-ttu-id="c5a65-130">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-130">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="c5a65-131">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-131">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="c5a65-132">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-132">Storage</span></span>
* <span data-ttu-id="c5a65-133">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-133">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="c5a65-134">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-134">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="c5a65-135">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="c5a65-135">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="c5a65-136">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="c5a65-136">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-137">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-137">VM</span></span>
* <span data-ttu-id="c5a65-138">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="c5a65-138">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="c5a65-139">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="c5a65-139">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="c5a65-140">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="c5a65-140">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="c5a65-141">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="c5a65-141">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="c5a65-142">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-142">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="c5a65-143">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="c5a65-143">Added `snapshot wait` command</span></span>
* <span data-ttu-id="c5a65-144">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-144">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="c5a65-145">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-145">November 6, 2018</span></span>

<span data-ttu-id="c5a65-146">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="c5a65-146">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-147">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-147">Core</span></span>
* <span data-ttu-id="c5a65-148">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="c5a65-148">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-149">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-149">ACR</span></span>
* <span data-ttu-id="c5a65-150">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="c5a65-150">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="c5a65-151">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="c5a65-151">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-152">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-152">ACS</span></span>
* <span data-ttu-id="c5a65-153">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-153">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="c5a65-154">Advisor</span><span class="sxs-lookup"><span data-stu-id="c5a65-154">Advisor</span></span>
* <span data-ttu-id="c5a65-155">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c5a65-155">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="c5a65-156">AMS</span><span class="sxs-lookup"><span data-stu-id="c5a65-156">AMS</span></span>
* <span data-ttu-id="c5a65-157">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="c5a65-157">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="c5a65-158">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="c5a65-158">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="c5a65-159">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-159">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="c5a65-160">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="c5a65-160">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="c5a65-161">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="c5a65-161">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="c5a65-162">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="c5a65-162">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="c5a65-163">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="c5a65-163">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="c5a65-164">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="c5a65-164">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="c5a65-165">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c5a65-165">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="c5a65-166">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c5a65-166">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="c5a65-167">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="c5a65-167">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="c5a65-168">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-168">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="c5a65-169">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="c5a65-169">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="c5a65-170">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="c5a65-170">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="c5a65-171">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-171">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="c5a65-172">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="c5a65-172">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="c5a65-173">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="c5a65-173">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-174">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-174">AppService</span></span>
* <span data-ttu-id="c5a65-175">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="c5a65-175">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="c5a65-176">Configuration</span><span class="sxs-lookup"><span data-stu-id="c5a65-176">Configure</span></span>
* <span data-ttu-id="c5a65-177">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="c5a65-177">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-178">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-178">Container</span></span>
* <span data-ttu-id="c5a65-179">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="c5a65-179">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="c5a65-180">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c5a65-180">EventHub</span></span>
* <span data-ttu-id="c5a65-181">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-181">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-182">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-182">Interactive</span></span>
* <span data-ttu-id="c5a65-183">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="c5a65-183">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-184">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-184">Monitor</span></span>
* <span data-ttu-id="c5a65-185">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-185">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-186">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-186">Network</span></span>
* <span data-ttu-id="c5a65-187">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="c5a65-187">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="c5a65-188">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-188">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="c5a65-189">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-189">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="c5a65-190">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-190">Profile</span></span>
* <span data-ttu-id="c5a65-191">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="c5a65-191">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-192">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-192">RDBMS</span></span>
* <span data-ttu-id="c5a65-193">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="c5a65-193">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-194">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-194">Resource</span></span>
* <span data-ttu-id="c5a65-195">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="c5a65-195">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-196">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-196">Role</span></span>
* <span data-ttu-id="c5a65-197">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="c5a65-197">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="c5a65-198">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="c5a65-198">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="c5a65-199">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="c5a65-199">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-200">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-200">Storage</span></span>
* <span data-ttu-id="c5a65-201">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="c5a65-201">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-202">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-202">VM</span></span>
* <span data-ttu-id="c5a65-203">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="c5a65-203">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="c5a65-204">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-204">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="c5a65-205">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="c5a65-205">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="c5a65-206">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="c5a65-206">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="c5a65-207">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="c5a65-207">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="c5a65-208">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="c5a65-208">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="c5a65-209">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-209">October 23, 2018</span></span>

<span data-ttu-id="c5a65-210">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="c5a65-210">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-211">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-211">Core</span></span>
* <span data-ttu-id="c5a65-212">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="c5a65-212">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="c5a65-213">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="c5a65-213">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-214">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-214">ACR</span></span>
* <span data-ttu-id="c5a65-215">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="c5a65-215">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="c5a65-216">CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-216">CDN</span></span>
* <span data-ttu-id="c5a65-217">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="c5a65-217">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c5a65-218">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c5a65-218">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-219">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-219">Container</span></span>
* <span data-ttu-id="c5a65-220">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="c5a65-220">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="c5a65-221">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-221">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="c5a65-222">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="c5a65-222">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="c5a65-223">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-223">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="c5a65-224">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c5a65-224">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="c5a65-225">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="c5a65-225">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="c5a65-226">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-226">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c5a65-227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-227">CosmosDB</span></span>
* <span data-ttu-id="c5a65-228">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-228">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-229">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-229">Interactive</span></span>
* <span data-ttu-id="c5a65-230">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="c5a65-230">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="c5a65-231">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c5a65-231">IoT Central</span></span>
* <span data-ttu-id="c5a65-232">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="c5a65-232">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="c5a65-233">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="c5a65-233">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-234">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-234">Monitor</span></span>
* <span data-ttu-id="c5a65-235">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="c5a65-235">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="c5a65-236">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-236">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="c5a65-237">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c5a65-237">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c5a65-238">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c5a65-238">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="c5a65-239">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="c5a65-239">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="c5a65-240">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c5a65-240">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="c5a65-241">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="c5a65-241">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="c5a65-242">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c5a65-242">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c5a65-243">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c5a65-243">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="c5a65-244">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-244">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-245">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-245">Network</span></span>
* <span data-ttu-id="c5a65-246">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-246">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="c5a65-247">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-247">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="c5a65-248">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c5a65-248">ServiceBus</span></span>
* <span data-ttu-id="c5a65-249">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="c5a65-249">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-250">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-250">SQL</span></span>
* <span data-ttu-id="c5a65-251">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c5a65-251">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-252">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-252">Storage</span></span>
* <span data-ttu-id="c5a65-253">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="c5a65-253">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="c5a65-254">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="c5a65-254">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-255">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-255">VM</span></span>
* <span data-ttu-id="c5a65-256">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-256">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="c5a65-257">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-257">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="c5a65-258">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-258">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="c5a65-259">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-259">October 16, 2018</span></span>

<span data-ttu-id="c5a65-260">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="c5a65-260">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-261">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-261">VM</span></span>
* <span data-ttu-id="c5a65-262">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="c5a65-262">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="c5a65-263">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-263">October 9, 2018</span></span>

<span data-ttu-id="c5a65-264">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="c5a65-264">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-265">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-265">Core</span></span>
* <span data-ttu-id="c5a65-266">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="c5a65-266">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-267">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-267">ACR</span></span>
* <span data-ttu-id="c5a65-268">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="c5a65-268">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-269">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-269">ACS</span></span>
* <span data-ttu-id="c5a65-270">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="c5a65-270">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="c5a65-271">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="c5a65-271">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="c5a65-272">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="c5a65-272">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="c5a65-273">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="c5a65-273">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-274">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-274">Container</span></span>
* <span data-ttu-id="c5a65-275">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="c5a65-275">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="c5a65-276">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-276">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="c5a65-277">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c5a65-277">Event Hub</span></span>
* <span data-ttu-id="c5a65-278">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-278">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="c5a65-279">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c5a65-279">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="c5a65-280">Extensions</span><span class="sxs-lookup"><span data-stu-id="c5a65-280">Extensions</span></span>
* <span data-ttu-id="c5a65-281">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="c5a65-281">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c5a65-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c5a65-282">HDInsight</span></span>
* <span data-ttu-id="c5a65-283">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-283">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-284">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-284">IoT</span></span>
* <span data-ttu-id="c5a65-285">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="c5a65-285">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-286">KeyVault</span></span>
* <span data-ttu-id="c5a65-287">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="c5a65-287">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-288">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-288">Network</span></span>
* <span data-ttu-id="c5a65-289">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="c5a65-289">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="c5a65-290">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="c5a65-290">See #6052</span></span>
* <span data-ttu-id="c5a65-291">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-291">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="c5a65-292">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="c5a65-292">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="c5a65-293">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c5a65-293">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="c5a65-294">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c5a65-294">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="c5a65-295">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="c5a65-295">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="c5a65-296">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-296">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-297">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-297">Role</span></span>
* <span data-ttu-id="c5a65-298">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="c5a65-298">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="c5a65-299">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="c5a65-299">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="c5a65-300">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="c5a65-300">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="c5a65-301">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="c5a65-301">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="c5a65-302">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c5a65-302">Service Bus</span></span>
* <span data-ttu-id="c5a65-303">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c5a65-303">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-304">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-304">VM</span></span>
* <span data-ttu-id="c5a65-305">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="c5a65-305">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="c5a65-306">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-306">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="c5a65-307">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="c5a65-307">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="c5a65-308">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="c5a65-308">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="c5a65-309">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-309">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="c5a65-310">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="c5a65-310">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="c5a65-311">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-311">September 21, 2018</span></span>

<span data-ttu-id="c5a65-312">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="c5a65-312">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-313">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-313">ACR</span></span>
* <span data-ttu-id="c5a65-314">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-314">Added ACR Task commands</span></span>
* <span data-ttu-id="c5a65-315">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="c5a65-315">Added quick run command</span></span>
* <span data-ttu-id="c5a65-316">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c5a65-316">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="c5a65-317">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-317">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="c5a65-318">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="c5a65-318">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="c5a65-319">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="c5a65-319">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-320">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-320">ACS</span></span>
* <span data-ttu-id="c5a65-321">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-321">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="c5a65-322">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="c5a65-322">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-323">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-323">AppService</span></span>

* <span data-ttu-id="c5a65-324">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="c5a65-324">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="c5a65-325">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="c5a65-325">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="c5a65-326">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="c5a65-326">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="c5a65-327">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="c5a65-327">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-328">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-328">Batch</span></span>
* <span data-ttu-id="c5a65-329">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="c5a65-329">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="c5a65-330">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="c5a65-330">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="c5a65-331">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-331">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="c5a65-332">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="c5a65-332">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c5a65-333">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-333">Batch AI</span></span> 
* <span data-ttu-id="c5a65-334">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-334">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c5a65-335">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-335">Cognitive Services</span></span>
* <span data-ttu-id="c5a65-336">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="c5a65-336">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="c5a65-337">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="c5a65-337">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="c5a65-338">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="c5a65-338">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="c5a65-339">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-339">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="c5a65-340">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c5a65-340">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="c5a65-341">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="c5a65-341">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-342">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-342">Container</span></span>
* <span data-ttu-id="c5a65-343">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="c5a65-343">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="c5a65-344">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-344">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="c5a65-345">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c5a65-345">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="c5a65-346">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-346">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="c5a65-347">DataLake</span><span class="sxs-lookup"><span data-stu-id="c5a65-347">Datalake</span></span>
* <span data-ttu-id="c5a65-348">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c5a65-348">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="c5a65-349">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="c5a65-349">Interactive Shell</span></span>
* <span data-ttu-id="c5a65-350">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-350">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="c5a65-351">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="c5a65-351">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-352">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-352">IoT</span></span>
* <span data-ttu-id="c5a65-353">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-353">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="c5a65-354">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c5a65-354">Key Vault</span></span>
* <span data-ttu-id="c5a65-355">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="c5a65-355">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-356">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-356">Network</span></span>
* <span data-ttu-id="c5a65-357">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-357">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="c5a65-358">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="c5a65-358">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="c5a65-359">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="c5a65-359">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="c5a65-360">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-360">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="c5a65-361">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-361">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="c5a65-362">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-362">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="c5a65-363">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-363">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="c5a65-364">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="c5a65-364">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="c5a65-365">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="c5a65-365">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="c5a65-366">`network express-route create/update` : ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="c5a65-366">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="c5a65-367">`network vnet subnet create/update` : ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="c5a65-367">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="c5a65-368">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="c5a65-368">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="c5a65-369">`network traffic-manager profile create/update` : ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="c5a65-369">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="c5a65-370">`network lb frontend-ip create/update` : correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="c5a65-370">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="c5a65-371">`dns record-set * create/update` : ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="c5a65-371">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="c5a65-372">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="c5a65-372">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="c5a65-373">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-373">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="c5a65-374">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="c5a65-374">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-375">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-375">RDBMS</span></span>
* <span data-ttu-id="c5a65-376">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-376">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="c5a65-377">Réservation</span><span class="sxs-lookup"><span data-stu-id="c5a65-377">Reservation</span></span>
* <span data-ttu-id="c5a65-378">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="c5a65-378">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="c5a65-379">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="c5a65-379">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="c5a65-380">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="c5a65-380">Manage App</span></span>
* <span data-ttu-id="c5a65-381">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="c5a65-381">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="c5a65-382">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="c5a65-382">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-383">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-383">Role</span></span>
* <span data-ttu-id="c5a65-384">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="c5a65-384">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="c5a65-385">SignalR</span><span class="sxs-lookup"><span data-stu-id="c5a65-385">SignalR</span></span>
* <span data-ttu-id="c5a65-386">Première version</span><span class="sxs-lookup"><span data-stu-id="c5a65-386">First release</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-387">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-387">Storage</span></span>
* <span data-ttu-id="c5a65-388">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="c5a65-388">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="c5a65-389">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="c5a65-389">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-390">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-390">VM</span></span>
* <span data-ttu-id="c5a65-391">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="c5a65-391">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="c5a65-392">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="c5a65-392">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="c5a65-393">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-393">August 28, 2018</span></span>

<span data-ttu-id="c5a65-394">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="c5a65-394">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-395">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-395">Core</span></span>

* <span data-ttu-id="c5a65-396">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="c5a65-396">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="c5a65-397">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c5a65-397">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-398">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-398">ACR</span></span>

* <span data-ttu-id="c5a65-399">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c5a65-399">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="c5a65-400">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="c5a65-400">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-401">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-401">ACS</span></span>

* <span data-ttu-id="c5a65-402">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="c5a65-402">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="c5a65-403">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="c5a65-403">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-404">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-404">AppService</span></span>

* <span data-ttu-id="c5a65-405">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="c5a65-405">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="c5a65-406">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="c5a65-406">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="c5a65-407">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-407">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="c5a65-408">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c5a65-408">Backup</span></span>

* <span data-ttu-id="c5a65-409">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-409">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="c5a65-410">Service de robot</span><span class="sxs-lookup"><span data-stu-id="c5a65-410">Bot Service</span></span>

* <span data-ttu-id="c5a65-411">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="c5a65-411">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c5a65-412">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-412">Cognitive Services</span></span>

* <span data-ttu-id="c5a65-413">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="c5a65-413">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-414">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-414">IoT</span></span>

* <span data-ttu-id="c5a65-415">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="c5a65-415">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-416">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-416">Monitor</span></span>

* <span data-ttu-id="c5a65-417">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="c5a65-417">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="c5a65-418">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="c5a65-418">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-419">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-419">Network</span></span>

* <span data-ttu-id="c5a65-420">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-420">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-421">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-421">Resource</span></span>

* <span data-ttu-id="c5a65-422">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-422">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-423">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-423">Storage</span></span>

* <span data-ttu-id="c5a65-424">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-424">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-425">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-425">VM</span></span>

* <span data-ttu-id="c5a65-426">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-426">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="c5a65-427">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-427">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="c5a65-428">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-428">Auguest 14, 2018</span></span>

<span data-ttu-id="c5a65-429">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="c5a65-429">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-430">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-430">Core</span></span>

* <span data-ttu-id="c5a65-431">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="c5a65-431">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="c5a65-432">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="c5a65-432">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="c5a65-433">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="c5a65-433">Telemetry</span></span>

* <span data-ttu-id="c5a65-434">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c5a65-434">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-435">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-435">ACR</span></span>

* <span data-ttu-id="c5a65-436">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="c5a65-436">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="c5a65-437">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c5a65-437">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-438">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-438">ACS</span></span>

* <span data-ttu-id="c5a65-439">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-439">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="c5a65-440">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-440">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="c5a65-441">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c5a65-441">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="c5a65-442">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c5a65-442">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="c5a65-443">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="c5a65-443">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="c5a65-444">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-444">AppService</span></span>

* <span data-ttu-id="c5a65-445">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c5a65-445">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="c5a65-446">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="c5a65-446">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="c5a65-447">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-447">BatchAI</span></span>

* <span data-ttu-id="c5a65-448">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="c5a65-448">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="c5a65-449">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-449">Container</span></span>

* <span data-ttu-id="c5a65-450">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-450">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="c5a65-451">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-451">IoT</span></span>

* <span data-ttu-id="c5a65-452">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="c5a65-452">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="c5a65-453">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="c5a65-453">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="c5a65-454">Iot Central</span><span class="sxs-lookup"><span data-stu-id="c5a65-454">Iot Central</span></span>

* <span data-ttu-id="c5a65-455">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="c5a65-455">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-456">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-456">KeyVault</span></span>


* <span data-ttu-id="c5a65-457">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="c5a65-457">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="c5a65-458">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-458">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="c5a65-459">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="c5a65-459">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="c5a65-460">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c5a65-460">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="c5a65-461">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c5a65-461">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="c5a65-462">Relais</span><span class="sxs-lookup"><span data-stu-id="c5a65-462">Relay</span></span>

* <span data-ttu-id="c5a65-463">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-463">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-464">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-464">Sql</span></span>

* <span data-ttu-id="c5a65-465">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="c5a65-465">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-466">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-466">Storage</span></span>

* <span data-ttu-id="c5a65-467">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="c5a65-467">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="c5a65-468">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="c5a65-468">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="c5a65-469">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="c5a65-469">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="c5a65-470">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="c5a65-470">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="c5a65-471">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-471">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-472">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-472">VM</span></span>

* <span data-ttu-id="c5a65-473">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="c5a65-473">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="c5a65-474">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-474">July 31, 2018</span></span>

<span data-ttu-id="c5a65-475">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="c5a65-475">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-476">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-476">ACR</span></span>

* <span data-ttu-id="c5a65-477">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-477">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="c5a65-478">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="c5a65-478">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-479">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-479">ACS</span></span>

* <span data-ttu-id="c5a65-480">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="c5a65-480">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-481">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-481">Batch</span></span>

* <span data-ttu-id="c5a65-482">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c5a65-482">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-483">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-483">Container</span></span>

* <span data-ttu-id="c5a65-484">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="c5a65-484">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-485">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-485">Network</span></span>

* <span data-ttu-id="c5a65-486">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c5a65-486">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="c5a65-487">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-487">Resource</span></span>

* <span data-ttu-id="c5a65-488">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c5a65-488">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="c5a65-489">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="c5a65-489">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-490">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-490">Role</span></span>

* <span data-ttu-id="c5a65-491">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-491">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="c5a65-492">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-492">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="c5a65-493">Recherche</span><span class="sxs-lookup"><span data-stu-id="c5a65-493">Search</span></span>

* <span data-ttu-id="c5a65-494">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="c5a65-494">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="c5a65-495">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c5a65-495">Service Bus</span></span>

* <span data-ttu-id="c5a65-496">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="c5a65-496">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="c5a65-497">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-497">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="c5a65-498">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="c5a65-498">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="c5a65-499">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-499">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-500">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-500">Storage</span></span>

* <span data-ttu-id="c5a65-501">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="c5a65-501">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="c5a65-502">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-502">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-503">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-503">VM</span></span>

* <span data-ttu-id="c5a65-504">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-504">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="c5a65-505">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="c5a65-505">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="c5a65-506">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="c5a65-506">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="c5a65-507">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-507">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="c5a65-508">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-508">July 18, 2018</span></span>

<span data-ttu-id="c5a65-509">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="c5a65-509">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-510">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-510">Core</span></span>

* <span data-ttu-id="c5a65-511">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="c5a65-511">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="c5a65-512">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c5a65-512">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="c5a65-513">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c5a65-513">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-514">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-514">ACR</span></span>

* <span data-ttu-id="c5a65-515">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="c5a65-515">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="c5a65-516">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="c5a65-516">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="c5a65-517">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="c5a65-517">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="c5a65-518">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="c5a65-518">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-519">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-519">ACS</span></span>

* <span data-ttu-id="c5a65-520">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="c5a65-520">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-521">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-521">AppService</span></span>

* <span data-ttu-id="c5a65-522">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="c5a65-522">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-523">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-523">Batch</span></span>

* <span data-ttu-id="c5a65-524">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c5a65-524">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="c5a65-525">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="c5a65-525">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c5a65-526">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-526">Batch AI</span></span>

* <span data-ttu-id="c5a65-527">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="c5a65-527">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-528">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-528">Container</span></span>

* <span data-ttu-id="c5a65-529">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="c5a65-529">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="c5a65-530">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="c5a65-530">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-531">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-531">Network</span></span>

* <span data-ttu-id="c5a65-532">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-532">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="c5a65-533">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="c5a65-533">Added `network nic wait`</span></span>
* <span data-ttu-id="c5a65-534">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-534">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="c5a65-535">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-535">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="c5a65-536">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-536">Resource</span></span>

* <span data-ttu-id="c5a65-537">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c5a65-537">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="c5a65-538">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c5a65-538">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="c5a65-539">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="c5a65-539">Added `deployment wait` command</span></span>
* <span data-ttu-id="c5a65-540">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="c5a65-540">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-541">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-541">SQL</span></span>

* <span data-ttu-id="c5a65-542">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-542">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="c5a65-543">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="c5a65-543">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="c5a65-544">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="c5a65-544">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-545">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-545">Storage</span></span>

* <span data-ttu-id="c5a65-546">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="c5a65-546">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-547">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-547">VM</span></span>

* <span data-ttu-id="c5a65-548">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-548">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="c5a65-549">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-549">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="c5a65-550">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="c5a65-550">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c5a65-551">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-551">July 3, 2018</span></span>

<span data-ttu-id="c5a65-552">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="c5a65-552">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="c5a65-553">AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-553">AKS</span></span>

* <span data-ttu-id="c5a65-554">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-554">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c5a65-555">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-555">July 3, 2018</span></span>

<span data-ttu-id="c5a65-556">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="c5a65-556">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-557">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-557">Core</span></span>

* <span data-ttu-id="c5a65-558">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-558">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-559">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-559">ACR</span></span>

* <span data-ttu-id="c5a65-560">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="c5a65-560">Added polling build status</span></span>
* <span data-ttu-id="c5a65-561">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="c5a65-561">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="c5a65-562">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c5a65-562">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-563">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-563">ACS</span></span>

* <span data-ttu-id="c5a65-564">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-564">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="c5a65-565">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-565">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="c5a65-566">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-566">Updated options for `aks browse` command.</span></span> <span data-ttu-id="c5a65-567">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="c5a65-567">Added `--listen-port` support</span></span>
* <span data-ttu-id="c5a65-568">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-568">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="c5a65-569">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="c5a65-569">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="c5a65-570">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="c5a65-570">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-571">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-571">AppService</span></span>

* <span data-ttu-id="c5a65-572">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="c5a65-572">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="c5a65-573">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="c5a65-573">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="c5a65-574">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c5a65-574">Backup</span></span>

* <span data-ttu-id="c5a65-575">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="c5a65-575">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="c5a65-576">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-576">BatchAI</span></span>

* <span data-ttu-id="c5a65-577">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-577">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="c5a65-578">Cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-578">Cloud</span></span>

* <span data-ttu-id="c5a65-579">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-579">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-580">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-580">Container</span></span>

* <span data-ttu-id="c5a65-581">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="c5a65-581">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="c5a65-582">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="c5a65-582">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="c5a65-583">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="c5a65-583">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-584">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-584">Extension</span></span>

* <span data-ttu-id="c5a65-585">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="c5a65-585">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-586">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-586">Network</span></span>

* <span data-ttu-id="c5a65-587">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="c5a65-587">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-588">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c5a65-588">Rdbms</span></span>

* <span data-ttu-id="c5a65-589">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c5a65-589">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-590">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-590">Resource</span></span>

* <span data-ttu-id="c5a65-591">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="c5a65-591">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-592">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-592">VM</span></span>

* <span data-ttu-id="c5a65-593">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="c5a65-593">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="c5a65-594">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-594">June 25, 2018</span></span>

<span data-ttu-id="c5a65-595">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="c5a65-595">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="c5a65-596">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-596">CLI</span></span>

* <span data-ttu-id="c5a65-597">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-597">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="c5a65-598">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-598">June 19, 2018</span></span>

<span data-ttu-id="c5a65-599">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="c5a65-599">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-600">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-600">Core</span></span>

* <span data-ttu-id="c5a65-601">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-601">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-602">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-602">ACR</span></span>

* <span data-ttu-id="c5a65-603">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="c5a65-603">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="c5a65-604">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-604">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-605">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-605">ACS</span></span>

* <span data-ttu-id="c5a65-606">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-606">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="c5a65-607">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-607">Added `--update` support</span></span>
* <span data-ttu-id="c5a65-608">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="c5a65-608">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="c5a65-609">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="c5a65-609">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="c5a65-610">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="c5a65-610">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="c5a65-611">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c5a65-611">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="c5a65-612">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c5a65-612">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="c5a65-613">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c5a65-613">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-614">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-614">AppService</span></span>

* <span data-ttu-id="c5a65-615">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="c5a65-615">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="c5a65-616">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c5a65-616">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-617">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-617">Batch</span></span>

* <span data-ttu-id="c5a65-618">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-618">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c5a65-619">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-619">Batch AI</span></span>

* <span data-ttu-id="c5a65-620">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="c5a65-620">Added support for workspaces.</span></span> <span data-ttu-id="c5a65-621">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="c5a65-621">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="c5a65-622">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="c5a65-622">Added support for experiments.</span></span> <span data-ttu-id="c5a65-623">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="c5a65-623">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="c5a65-624">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="c5a65-624">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="c5a65-625">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-625">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="c5a65-626">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="c5a65-626">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="c5a65-627">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="c5a65-627">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="c5a65-628">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-628">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="c5a65-629">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="c5a65-629">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="c5a65-630">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-630">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="c5a65-631">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="c5a65-631">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="c5a65-632">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-632">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="c5a65-633">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="c5a65-633">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="c5a65-634">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="c5a65-634">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="c5a65-635">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="c5a65-635">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="c5a65-636">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-636">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="c5a65-637">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="c5a65-637">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="c5a65-638">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="c5a65-638">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="c5a65-639">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c5a65-639">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c5a65-640">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c5a65-640">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c5a65-641">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="c5a65-641">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="c5a65-642">Cartes</span><span class="sxs-lookup"><span data-stu-id="c5a65-642">Maps</span></span>

* <span data-ttu-id="c5a65-643">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="c5a65-643">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-644">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-644">Network</span></span>

* <span data-ttu-id="c5a65-645">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="c5a65-645">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="c5a65-646">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="c5a65-646">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="c5a65-647">#6502</span><span class="sxs-lookup"><span data-stu-id="c5a65-647">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="c5a65-648">Réservations</span><span class="sxs-lookup"><span data-stu-id="c5a65-648">Reservations</span></span>

* <span data-ttu-id="c5a65-649">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-649">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="c5a65-650">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-650">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="c5a65-651">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="c5a65-651">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="c5a65-652">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c5a65-652">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="c5a65-653">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c5a65-653">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="c5a65-654">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-654">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-655">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-655">Role</span></span>

* <span data-ttu-id="c5a65-656">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-656">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-657">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-657">SQL</span></span>

* <span data-ttu-id="c5a65-658">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-658">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-659">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-659">Storage</span></span>

* <span data-ttu-id="c5a65-660">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="c5a65-660">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-661">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-661">VM</span></span>

* <span data-ttu-id="c5a65-662">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-662">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="c5a65-663">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="c5a65-663">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="c5a65-664">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="c5a65-664">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c5a65-665">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-665">June 13, 2018</span></span>

<span data-ttu-id="c5a65-666">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="c5a65-666">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-667">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-667">Core</span></span>

* <span data-ttu-id="c5a65-668">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-668">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c5a65-669">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-669">June 13, 2018</span></span>

<span data-ttu-id="c5a65-670">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="c5a65-670">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="c5a65-671">AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-671">AKS</span></span>

* <span data-ttu-id="c5a65-672">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-672">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="c5a65-673">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="c5a65-673">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="c5a65-674">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-674">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="c5a65-675">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-675">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="c5a65-676">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-676">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-677">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-677">AppService</span></span>

* <span data-ttu-id="c5a65-678">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="c5a65-678">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c5a65-679">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-679">June 5, 2018</span></span>

<span data-ttu-id="c5a65-680">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="c5a65-680">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-681">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-681">Interactive</span></span>

* <span data-ttu-id="c5a65-682">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c5a65-682">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c5a65-683">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-683">June 5, 2018</span></span>

<span data-ttu-id="c5a65-684">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="c5a65-684">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-685">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-685">Core</span></span>

* <span data-ttu-id="c5a65-686">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="c5a65-686">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="c5a65-687">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c5a65-687">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-688">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-688">ACR</span></span>

* <span data-ttu-id="c5a65-689">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="c5a65-689">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="c5a65-690">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="c5a65-690">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="c5a65-691">AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-691">AKS</span></span>

* <span data-ttu-id="c5a65-692">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="c5a65-692">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-693">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-693">Batch</span></span>

* <span data-ttu-id="c5a65-694">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="c5a65-694">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-695">IOT</span><span class="sxs-lookup"><span data-stu-id="c5a65-695">IOT</span></span>

* <span data-ttu-id="c5a65-696">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="c5a65-696">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-697">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-697">Network</span></span>

* <span data-ttu-id="c5a65-698">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="c5a65-698">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c5a65-699">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c5a65-699">Policy Insights</span></span>

* <span data-ttu-id="c5a65-700">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-700">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="c5a65-701">ARM</span><span class="sxs-lookup"><span data-stu-id="c5a65-701">ARM</span></span>

* <span data-ttu-id="c5a65-702">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-702">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-703">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-703">SQL</span></span>

* <span data-ttu-id="c5a65-704">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="c5a65-704">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="c5a65-705">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="c5a65-705">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="c5a65-706">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-706">Storage</span></span>

* <span data-ttu-id="c5a65-707">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="c5a65-707">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-708">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-708">VM</span></span>

* <span data-ttu-id="c5a65-709">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="c5a65-709">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="c5a65-710">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-710">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="c5a65-711">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-711">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="c5a65-712">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-712">May 22, 2018</span></span>

<span data-ttu-id="c5a65-713">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="c5a65-713">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-714">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-714">Core</span></span>

* <span data-ttu-id="c5a65-715">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="c5a65-715">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-716">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-716">ACS</span></span>

* <span data-ttu-id="c5a65-717">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="c5a65-717">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="c5a65-718">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="c5a65-718">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-719">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-719">AppService</span></span>

* <span data-ttu-id="c5a65-720">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c5a65-720">Improved generic update commands</span></span>
* <span data-ttu-id="c5a65-721">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="c5a65-721">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-722">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-722">Container</span></span>

* <span data-ttu-id="c5a65-723">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="c5a65-723">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="c5a65-724">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-724">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-725">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-725">Extension</span></span>

* <span data-ttu-id="c5a65-726">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="c5a65-726">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-727">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-727">Interactive</span></span>

* <span data-ttu-id="c5a65-728">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-728">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="c5a65-729">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="c5a65-729">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-730">KeyVault</span></span>

* <span data-ttu-id="c5a65-731">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c5a65-731">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-732">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-732">Network</span></span>

* <span data-ttu-id="c5a65-733">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="c5a65-733">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="c5a65-734">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="c5a65-734">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-735">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-735">SQL</span></span>

* <span data-ttu-id="c5a65-736">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="c5a65-736">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="c5a65-737">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="c5a65-737">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="c5a65-738">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="c5a65-738">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="c5a65-739">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c5a65-739">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="c5a65-740">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c5a65-740">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="c5a65-741">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-741">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="c5a65-742">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-742">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="c5a65-743">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-743">`edition`.</span></span> <span data-ttu-id="c5a65-744">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="c5a65-744">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="c5a65-745">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-745">`elasticPoolName`.</span></span> <span data-ttu-id="c5a65-746">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="c5a65-746">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="c5a65-747">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c5a65-747">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="c5a65-748">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-748">`edition`.</span></span> <span data-ttu-id="c5a65-749">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="c5a65-749">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="c5a65-750">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-750">`dtu`.</span></span> <span data-ttu-id="c5a65-751">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="c5a65-751">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="c5a65-752">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-752">`databaseDtuMin`.</span></span> <span data-ttu-id="c5a65-753">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="c5a65-753">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="c5a65-754">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-754">`databaseDtuMax`.</span></span> <span data-ttu-id="c5a65-755">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="c5a65-755">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="c5a65-756">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c5a65-756">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="c5a65-757">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c5a65-757">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-758">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-758">Storage</span></span>

* <span data-ttu-id="c5a65-759">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-759">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="c5a65-760">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="c5a65-760">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-761">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-761">VM</span></span>

* <span data-ttu-id="c5a65-762">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-762">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="c5a65-763">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="c5a65-763">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="c5a65-764">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="c5a65-764">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="c5a65-765">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="c5a65-765">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="c5a65-766">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-766">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="c5a65-767">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-767">May 7, 2018</span></span>

<span data-ttu-id="c5a65-768">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="c5a65-768">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-769">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-769">Core</span></span>

* <span data-ttu-id="c5a65-770">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="c5a65-770">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="c5a65-771">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="c5a65-771">Added limited support for positional arguments</span></span>
* <span data-ttu-id="c5a65-772">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-772">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="c5a65-773">#5591</span><span class="sxs-lookup"><span data-stu-id="c5a65-773">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="c5a65-774">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-774">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="c5a65-775">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="c5a65-775">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="c5a65-776">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-776">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="c5a65-777">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="c5a65-777">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="c5a65-778">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-778">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-779">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-779">ACR</span></span>

* <span data-ttu-id="c5a65-780">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-780">Added ACR Build commands</span></span>
* <span data-ttu-id="c5a65-781">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="c5a65-781">Improved resource not found error messages</span></span>
* <span data-ttu-id="c5a65-782">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-782">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="c5a65-783">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="c5a65-783">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="c5a65-784">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="c5a65-784">Improved repository commands error messages</span></span>
* <span data-ttu-id="c5a65-785">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="c5a65-785">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-786">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-786">ACS</span></span>

* <span data-ttu-id="c5a65-787">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="c5a65-787">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="c5a65-788">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c5a65-788">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="c5a65-789">AMS</span><span class="sxs-lookup"><span data-stu-id="c5a65-789">AMS</span></span>

* <span data-ttu-id="c5a65-790">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-790">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-791">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-791">Appservice</span></span>

* <span data-ttu-id="c5a65-792">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="c5a65-792">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="c5a65-793">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-793">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="c5a65-794">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="c5a65-794">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="c5a65-795">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-795">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c5a65-796">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-796">Batch AI</span></span>

* <span data-ttu-id="c5a65-797">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="c5a65-797">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c5a65-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-798">Cognitive Services</span></span>

* <span data-ttu-id="c5a65-799">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="c5a65-799">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="c5a65-800">Consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-800">Consumption</span></span>

* <span data-ttu-id="c5a65-801">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="c5a65-801">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-802">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-802">Container</span></span>

* <span data-ttu-id="c5a65-803">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="c5a65-803">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c5a65-804">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c5a65-804">Cosmos DB</span></span>

* <span data-ttu-id="c5a65-805">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c5a65-805">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="c5a65-806">DMS</span><span class="sxs-lookup"><span data-stu-id="c5a65-806">DMS</span></span>

* <span data-ttu-id="c5a65-807">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="c5a65-807">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-808">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-808">Extension</span></span>

* <span data-ttu-id="c5a65-809">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="c5a65-809">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-810">Interactive</span></span>

* <span data-ttu-id="c5a65-811">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="c5a65-811">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="c5a65-812">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="c5a65-812">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="c5a65-813">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="c5a65-813">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="c5a65-814">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-814">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="c5a65-815">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-815">Lab</span></span>

* <span data-ttu-id="c5a65-816">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="c5a65-816">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-817">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-817">Network</span></span>

* <span data-ttu-id="c5a65-818">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="c5a65-818">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="c5a65-819">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-819">Profile</span></span>

* <span data-ttu-id="c5a65-820">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-820">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="c5a65-821">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="c5a65-821">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="c5a65-822">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="c5a65-822">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="c5a65-823">Redis</span><span class="sxs-lookup"><span data-stu-id="c5a65-823">Redis</span></span>

* <span data-ttu-id="c5a65-824">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-824">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="c5a65-825">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="c5a65-825">Deprecated `redis list-all`.</span></span> <span data-ttu-id="c5a65-826">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-826">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="c5a65-827">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="c5a65-827">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="c5a65-828">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-828">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-829">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-829">Role</span></span>

* <span data-ttu-id="c5a65-830">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c5a65-830">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-831">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-831">Storage</span></span>

* <span data-ttu-id="c5a65-832">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="c5a65-832">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="c5a65-833">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="c5a65-833">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="c5a65-834">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="c5a65-834">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="c5a65-835">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="c5a65-835">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="c5a65-836">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-836">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-837">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-837">VM</span></span>

* <span data-ttu-id="c5a65-838">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="c5a65-838">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="c5a65-839">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c5a65-839">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="c5a65-840">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="c5a65-840">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="c5a65-841">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="c5a65-841">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="c5a65-842">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="c5a65-842">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="c5a65-843">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="c5a65-843">Added write accelerator support</span></span>
* <span data-ttu-id="c5a65-844">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c5a65-844">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="c5a65-845">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-845">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="c5a65-846">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="c5a65-846">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="c5a65-847">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-847">April 10, 2018</span></span>

<span data-ttu-id="c5a65-848">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="c5a65-848">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-849">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-849">ACR</span></span>

* <span data-ttu-id="c5a65-850">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="c5a65-850">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-851">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-851">ACS</span></span>

* <span data-ttu-id="c5a65-852">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="c5a65-852">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-853">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-853">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="c5a65-855">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="c5a65-855">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="c5a65-856">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-856">BatchAI</span></span>

* <span data-ttu-id="c5a65-857">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="c5a65-857">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="c5a65-858">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-858">Job level mounting</span></span>
  - <span data-ttu-id="c5a65-859">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="c5a65-859">Environment variables with secret values</span></span>
  - <span data-ttu-id="c5a65-860">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="c5a65-860">Performance counters settings</span></span>
  - <span data-ttu-id="c5a65-861">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-861">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="c5a65-862">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="c5a65-862">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="c5a65-863">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="c5a65-863">Usage and limits reporting</span></span>
  - <span data-ttu-id="c5a65-864">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="c5a65-864">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="c5a65-865">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="c5a65-865">Support for custom images</span></span>
  - <span data-ttu-id="c5a65-866">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="c5a65-866">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="c5a65-867">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-867">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="c5a65-868">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="c5a65-868">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="c5a65-869">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="c5a65-869">National clouds are supported</span></span>
* <span data-ttu-id="c5a65-870">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="c5a65-870">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="c5a65-871">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="c5a65-871">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="c5a65-872">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-872">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="c5a65-873">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="c5a65-873">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="c5a65-874">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="c5a65-874">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="c5a65-875">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="c5a65-875">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="c5a65-876">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-876">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="c5a65-877">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="c5a65-877">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="c5a65-878">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="c5a65-878">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="c5a65-879">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-879">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="c5a65-880">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-880">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="c5a65-881">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="c5a65-881">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="c5a65-882">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-882">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="c5a65-883">Facturation</span><span class="sxs-lookup"><span data-stu-id="c5a65-883">Billing</span></span>

* <span data-ttu-id="c5a65-884">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="c5a65-884">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="c5a65-885">Consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-885">Consumption</span></span>

* <span data-ttu-id="c5a65-886">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="c5a65-886">Added `marketplace` commands</span></span>
* <span data-ttu-id="c5a65-887">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c5a65-887">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="c5a65-888">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="c5a65-888">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="c5a65-889">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="c5a65-889">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="c5a65-890">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c5a65-890">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="c5a65-891">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="c5a65-891">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-892">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-892">Container</span></span>

* <span data-ttu-id="c5a65-893">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="c5a65-893">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="c5a65-894">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="c5a65-894">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-895">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-895">Extension</span></span>

* <span data-ttu-id="c5a65-896">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="c5a65-896">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-897">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-897">Interactive</span></span>

* <span data-ttu-id="c5a65-898">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="c5a65-898">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="c5a65-899">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-899">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="c5a65-900">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="c5a65-900">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-901">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-901">Network</span></span>

* <span data-ttu-id="c5a65-902">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="c5a65-902">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="c5a65-903">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-903">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="c5a65-904">#4910</span><span class="sxs-lookup"><span data-stu-id="c5a65-904">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="c5a65-905">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c5a65-905">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="c5a65-906">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c5a65-906">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="c5a65-907">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-907">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="c5a65-908">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-908">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="c5a65-909">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="c5a65-909">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-910">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-910">Profile</span></span>

* <span data-ttu-id="c5a65-911">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-911">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="c5a65-912">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="c5a65-912">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-913">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-913">RDBMS</span></span>

* <span data-ttu-id="c5a65-914">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="c5a65-914">Added `georestore` command</span></span>
* <span data-ttu-id="c5a65-915">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-915">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-916">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-916">Resource</span></span>

* <span data-ttu-id="c5a65-917">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-917">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="c5a65-918">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-918">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-919">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-919">SQL</span></span>

* <span data-ttu-id="c5a65-920">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="c5a65-920">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-921">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-921">Storage</span></span>

* <span data-ttu-id="c5a65-922">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="c5a65-922">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-923">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-923">VM</span></span>

* <span data-ttu-id="c5a65-924">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-924">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="c5a65-925">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="c5a65-925">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="c5a65-927">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-927">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="c5a65-928">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="c5a65-928">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="c5a65-929">#5718</span><span class="sxs-lookup"><span data-stu-id="c5a65-929">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="c5a65-930">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="c5a65-930">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="c5a65-931">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-931">March 27, 2018</span></span>

<span data-ttu-id="c5a65-932">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="c5a65-932">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-933">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-933">Core</span></span>

* <span data-ttu-id="c5a65-934">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="c5a65-934">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-935">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-935">ACS</span></span>

* <span data-ttu-id="c5a65-936">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c5a65-936">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-937">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-937">Appservice</span></span>

* <span data-ttu-id="c5a65-938">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-938">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="c5a65-939">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-939">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c5a65-940">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c5a65-940">Backup</span></span>

* <span data-ttu-id="c5a65-941">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="c5a65-941">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="c5a65-942">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-942">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="c5a65-943">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c5a65-943">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="c5a65-944">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-944">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-945">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-945">Container</span></span>

* <span data-ttu-id="c5a65-946">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="c5a65-946">Added `container exec` command.</span></span> <span data-ttu-id="c5a65-947">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="c5a65-947">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="c5a65-948">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-948">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-949">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-949">Extension</span></span>

* <span data-ttu-id="c5a65-950">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="c5a65-950">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="c5a65-951">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="c5a65-951">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="c5a65-952">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-952">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-953">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-953">Interactive</span></span>

* <span data-ttu-id="c5a65-954">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-954">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="c5a65-955">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="c5a65-955">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="c5a65-956">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="c5a65-956">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="c5a65-957">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="c5a65-957">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="c5a65-958">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-958">Lab</span></span>

* <span data-ttu-id="c5a65-959">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="c5a65-959">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-960">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-960">Monitor</span></span>

* <span data-ttu-id="c5a65-961">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c5a65-961">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="c5a65-962">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="c5a65-962">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="c5a65-963">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c5a65-963">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-964">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-964">Network</span></span>

* <span data-ttu-id="c5a65-965">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c5a65-965">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-966">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-966">Profile</span></span>

* <span data-ttu-id="c5a65-967">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="c5a65-967">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-968">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-968">RDBMS</span></span>

* <span data-ttu-id="c5a65-969">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="c5a65-969">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-970">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-970">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="c5a65-972">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-972">Role</span></span>

* <span data-ttu-id="c5a65-973">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-973">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="c5a65-974">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="c5a65-974">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="c5a65-975">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-975">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="c5a65-976">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-976">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="c5a65-977">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="c5a65-977">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-978">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-978">Storage</span></span>

* <span data-ttu-id="c5a65-979">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="c5a65-979">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="c5a65-980">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="c5a65-980">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-981">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-981">VM</span></span>

* <span data-ttu-id="c5a65-982">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="c5a65-982">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="c5a65-983">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-983">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="c5a65-984">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c5a65-984">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="c5a65-985">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="c5a65-985">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="c5a65-986">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-986">March 13, 2018</span></span>

<span data-ttu-id="c5a65-987">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="c5a65-987">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-988">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-988">ACR</span></span>

* <span data-ttu-id="c5a65-989">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="c5a65-989">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="c5a65-990">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="c5a65-990">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="c5a65-991">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="c5a65-991">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-992">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-992">ACS</span></span>

* <span data-ttu-id="c5a65-993">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="c5a65-993">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="c5a65-994">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="c5a65-994">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="c5a65-995">Advisor</span><span class="sxs-lookup"><span data-stu-id="c5a65-995">Advisor</span></span>

* <span data-ttu-id="c5a65-996">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-996">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="c5a65-997">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-997">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="c5a65-998">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="c5a65-998">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="c5a65-999">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-999">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="c5a65-1000">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1000">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1001">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1001">Appservice</span></span>

* <span data-ttu-id="c5a65-1002">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c5a65-1002">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="c5a65-1003">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1003">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c5a65-1004">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1004">Eventhubs</span></span>

* <span data-ttu-id="c5a65-1005">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1005">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-1006">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-1006">Extension</span></span>

* <span data-ttu-id="c5a65-1007">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1007">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-1008">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-1008">Interactive</span></span>

* <span data-ttu-id="c5a65-1009">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="c5a65-1009">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="c5a65-1010">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1010">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="c5a65-1011">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="c5a65-1011">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="c5a65-1012">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="c5a65-1012">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1013">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1013">Monitor</span></span>

* <span data-ttu-id="c5a65-1014">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1014">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="c5a65-1015">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1015">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="c5a65-1016">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1016">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="c5a65-1017">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1017">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1018">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1018">Network</span></span>

* <span data-ttu-id="c5a65-1019">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1019">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="c5a65-1020">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1020">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="c5a65-1021">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1021">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="c5a65-1022">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1022">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1023">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1023">Profile</span></span>

* <span data-ttu-id="c5a65-1024">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1024">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="c5a65-1025">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1025">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-1026">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1026">RDBMS</span></span>

* <span data-ttu-id="c5a65-1027">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="c5a65-1027">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="c5a65-1028">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c5a65-1028">Service Bus</span></span>

* <span data-ttu-id="c5a65-1029">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1029">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1030">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1030">Storage</span></span>

* <span data-ttu-id="c5a65-1031">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="c5a65-1031">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="c5a65-1032">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="c5a65-1032">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1033">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1033">VM</span></span>

* <span data-ttu-id="c5a65-1034">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="c5a65-1034">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="c5a65-1035">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1035">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="c5a65-1036">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1036">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="c5a65-1037">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="c5a65-1037">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="c5a65-1038">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-1038">February 27, 2018</span></span>

<span data-ttu-id="c5a65-1039">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="c5a65-1039">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1040">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1040">Core</span></span>

* <span data-ttu-id="c5a65-1041">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="c5a65-1041">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="c5a65-1042">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1042">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="c5a65-1043">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1043">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1044">ACS</span></span>

* <span data-ttu-id="c5a65-1045">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1045">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="c5a65-1046">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1046">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="c5a65-1047">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1047">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="c5a65-1048">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1048">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1049">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1049">Appservice</span></span>

* <span data-ttu-id="c5a65-1050">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1050">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="c5a65-1051">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="c5a65-1051">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c5a65-1052">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-1052">Cognitive Services</span></span>

* <span data-ttu-id="c5a65-1053">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-1053">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="c5a65-1054">Consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1054">Consumption</span></span>

* <span data-ttu-id="c5a65-1055">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="c5a65-1055">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="c5a65-1056">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1056">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1057">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1057">Container</span></span>

* <span data-ttu-id="c5a65-1058">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1058">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1059">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1059">Network</span></span>

* <span data-ttu-id="c5a65-1060">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1060">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1061">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1061">Resource</span></span>

* <span data-ttu-id="c5a65-1062">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="c5a65-1062">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1063">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1063">Role</span></span>

* <span data-ttu-id="c5a65-1064">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="c5a65-1064">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1065">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1065">SQL</span></span>

* <span data-ttu-id="c5a65-1066">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="c5a65-1066">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1067">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1067">Storage</span></span>

* <span data-ttu-id="c5a65-1068">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1068">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1069">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1069">VM</span></span>

* <span data-ttu-id="c5a65-1070">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="c5a65-1070">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="c5a65-1071">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-1071">February 13, 2018</span></span>

<span data-ttu-id="c5a65-1072">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="c5a65-1072">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1073">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1073">Core</span></span>

* <span data-ttu-id="c5a65-1074">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1074">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1075">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1075">ACS</span></span>

* <span data-ttu-id="c5a65-1076">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="c5a65-1076">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="c5a65-1077">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1077">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="c5a65-1078">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1078">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="c5a65-1079">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1079">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="c5a65-1080">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1080">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="c5a65-1081">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1081">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="c5a65-1082">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1082">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="c5a65-1083">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1083">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1084">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1084">Appservice</span></span>

* <span data-ttu-id="c5a65-1085">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="c5a65-1085">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="c5a65-1086">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1086">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="c5a65-1087">CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1087">CDN</span></span>

* <span data-ttu-id="c5a65-1088">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1088">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1089">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1089">Container</span></span>

* <span data-ttu-id="c5a65-1090">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="c5a65-1090">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="c5a65-1091">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1091">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c5a65-1092">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-1092">CosmosDB</span></span>

* <span data-ttu-id="c5a65-1093">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c5a65-1093">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-1094">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-1094">Extension</span></span>

* <span data-ttu-id="c5a65-1095">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1095">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="c5a65-1096">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1096">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="c5a65-1097">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c5a65-1097">Feedback</span></span>

* <span data-ttu-id="c5a65-1098">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c5a65-1098">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-1099">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-1099">Interactive</span></span>

* <span data-ttu-id="c5a65-1100">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c5a65-1100">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="c5a65-1101">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="c5a65-1101">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-1102">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1102">IoT</span></span>

* <span data-ttu-id="c5a65-1103">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c5a65-1103">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c5a65-1104">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c5a65-1104">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c5a65-1105">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1105">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="c5a65-1106">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="c5a65-1106">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1107">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1107">Monitor</span></span>

* <span data-ttu-id="c5a65-1108">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1108">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1109">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1109">Network</span></span>

* <span data-ttu-id="c5a65-1110">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1110">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="c5a65-1111">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1111">Profile</span></span>

* <span data-ttu-id="c5a65-1112">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1112">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1113">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1113">Resource</span></span>

* <span data-ttu-id="c5a65-1114">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1114">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1115">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1115">Role</span></span>

* <span data-ttu-id="c5a65-1116">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1116">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1117">SQL</span></span>

* <span data-ttu-id="c5a65-1118">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1118">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="c5a65-1119">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1119">Added `sql db rename`</span></span>
* <span data-ttu-id="c5a65-1120">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="c5a65-1120">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1121">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1121">Storage</span></span>

* <span data-ttu-id="c5a65-1122">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="c5a65-1122">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1123">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1123">VM</span></span>

* <span data-ttu-id="c5a65-1124">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1124">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="c5a65-1125">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1125">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="c5a65-1126">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1126">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="c5a65-1127">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-1127">January 31, 2018</span></span>

<span data-ttu-id="c5a65-1128">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="c5a65-1128">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1129">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1129">Core</span></span>

* <span data-ttu-id="c5a65-1130">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1130">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="c5a65-1131">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-1131">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="c5a65-1132">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1132">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="c5a65-1133">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="c5a65-1133">Use `--verbose` to see</span></span>
* <span data-ttu-id="c5a65-1134">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="c5a65-1134">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1135">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1135">ACS</span></span>

* <span data-ttu-id="c5a65-1136">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1136">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="c5a65-1137">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1137">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1138">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1138">Appservice</span></span>

* <span data-ttu-id="c5a65-1139">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1139">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="c5a65-1140">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="c5a65-1140">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="c5a65-1141">CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1141">CDN</span></span>

* <span data-ttu-id="c5a65-1142">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1142">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c5a65-1143">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-1143">CosmosDB</span></span>

* <span data-ttu-id="c5a65-1144">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1144">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-1145">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-1145">Interactive</span></span>

* <span data-ttu-id="c5a65-1146">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="c5a65-1146">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1147">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1147">Network</span></span>

* <span data-ttu-id="c5a65-1148">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1148">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="c5a65-1149">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1149">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="c5a65-1150">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1150">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="c5a65-1151">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1151">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="c5a65-1152">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1152">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="c5a65-1153">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1153">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="c5a65-1154">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1154">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="c5a65-1155">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1155">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="c5a65-1156">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1156">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="c5a65-1157">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1157">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1158">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1158">Profile</span></span>

* <span data-ttu-id="c5a65-1159">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c5a65-1159">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1160">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1160">Resource</span></span>

* <span data-ttu-id="c5a65-1161">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="c5a65-1161">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1162">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1162">Storage</span></span>

* <span data-ttu-id="c5a65-1163">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="c5a65-1163">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="c5a65-1164">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1164">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="c5a65-1165">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1165">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="c5a65-1166">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1166">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="c5a65-1167">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="c5a65-1167">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1168">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1168">VM</span></span>

* <span data-ttu-id="c5a65-1169">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="c5a65-1169">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="c5a65-1170">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1170">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="c5a65-1171">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="c5a65-1171">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="c5a65-1172">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1172">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="c5a65-1173">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c5a65-1173">January 17, 2018</span></span>

<span data-ttu-id="c5a65-1174">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="c5a65-1174">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1175">ACR</span></span>

* <span data-ttu-id="c5a65-1176">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-1176">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="c5a65-1177">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="c5a65-1177">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1178">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1178">ACS</span></span>

* <span data-ttu-id="c5a65-1179">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1179">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="c5a65-1180">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1180">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1181">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1181">Appservice</span></span>

* <span data-ttu-id="c5a65-1182">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="c5a65-1182">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="c5a65-1183">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1183">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="c5a65-1184">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1184">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="c5a65-1185">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c5a65-1185">Backup</span></span>

* <span data-ttu-id="c5a65-1186">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="c5a65-1186">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="c5a65-1187">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1187">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="c5a65-1188">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="c5a65-1188">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="c5a65-1189">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="c5a65-1189">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="c5a65-1190">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1190">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-1191">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1191">Batch</span></span>

* <span data-ttu-id="c5a65-1192">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="c5a65-1192">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="c5a65-1193">Cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-1193">Cloud</span></span>

* <span data-ttu-id="c5a65-1194">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-1194">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="c5a65-1195">Consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1195">Consumption</span></span>

* <span data-ttu-id="c5a65-1196">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1196">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="c5a65-1197">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c5a65-1197">Event Grid</span></span>

* <span data-ttu-id="c5a65-1198">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1198">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c5a65-1199">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1199">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c5a65-1200">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1200">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="c5a65-1201">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="c5a65-1201">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="c5a65-1202">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1202">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="c5a65-1203">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1203">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="c5a65-1204">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1204">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="c5a65-1205">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="c5a65-1205">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-1206">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-1206">Interactive</span></span>

* <span data-ttu-id="c5a65-1207">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="c5a65-1207">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="c5a65-1208">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1208">Fixed errors on startup</span></span>
* <span data-ttu-id="c5a65-1209">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1209">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-1210">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1210">IoT</span></span>

* <span data-ttu-id="c5a65-1211">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="c5a65-1211">Added support for device provisioning service</span></span>
* <span data-ttu-id="c5a65-1212">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1212">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="c5a65-1213">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1213">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1214">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1214">Monitor</span></span>

* <span data-ttu-id="c5a65-1215">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1215">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="c5a65-1216">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1216">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="c5a65-1217">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="c5a65-1217">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1218">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1218">Network</span></span>

* <span data-ttu-id="c5a65-1219">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1219">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="c5a65-1220">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1220">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1221">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1221">Profile</span></span>

* <span data-ttu-id="c5a65-1222">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1222">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1223">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1223">Role</span></span>

* <span data-ttu-id="c5a65-1224">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="c5a65-1224">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c5a65-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c5a65-1225">Service Fabric</span></span>

* <span data-ttu-id="c5a65-1226">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="c5a65-1226">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="c5a65-1227">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1227">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1228">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1228">VM</span></span>

* <span data-ttu-id="c5a65-1229">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1229">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="c5a65-1230">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1230">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="c5a65-1231">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1231">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="c5a65-1232">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1232">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="c5a65-1233">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="c5a65-1233">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="c5a65-1234">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1234">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c5a65-1235">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1235">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="c5a65-1236">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1236">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="c5a65-1237">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1237">December 19, 2017</span></span>

<span data-ttu-id="c5a65-1238">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="c5a65-1238">Version 2.0.23</span></span>

* <span data-ttu-id="c5a65-1239">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1239">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1240">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1240">Container</span></span>

* <span data-ttu-id="c5a65-1241">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1241">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1242">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1242">Network</span></span>

* <span data-ttu-id="c5a65-1243">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1243">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="c5a65-1244">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1244">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1245">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1245">Storage</span></span>

* <span data-ttu-id="c5a65-1246">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="c5a65-1246">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1247">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1247">VM</span></span>

* <span data-ttu-id="c5a65-1248">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1248">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="c5a65-1249">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1249">December 5, 2017</span></span>

<span data-ttu-id="c5a65-1250">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="c5a65-1250">Version 2.0.22</span></span>

* <span data-ttu-id="c5a65-1251">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1251">Removed `az component` commands.</span></span> <span data-ttu-id="c5a65-1252">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="c5a65-1252">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1253">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1253">Core</span></span>
* <span data-ttu-id="c5a65-1254">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="c5a65-1254">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="c5a65-1255">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1255">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1256">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1256">ACS</span></span>

* <span data-ttu-id="c5a65-1257">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1257">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="c5a65-1258">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1258">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="c5a65-1259">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="c5a65-1259">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="c5a65-1260">Advisor</span><span class="sxs-lookup"><span data-stu-id="c5a65-1260">Advisor</span></span>

* <span data-ttu-id="c5a65-1261">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1261">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1262">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1262">Appservice</span></span>

* <span data-ttu-id="c5a65-1263">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1263">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="c5a65-1264">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1264">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="c5a65-1265">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1265">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="c5a65-1266">Consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1266">Consumption</span></span>

* <span data-ttu-id="c5a65-1267">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="c5a65-1267">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1268">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1268">Container</span></span>

* <span data-ttu-id="c5a65-1269">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1269">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1270">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1270">Monitor</span></span>

* <span data-ttu-id="c5a65-1271">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="c5a65-1271">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1272">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1272">Resource</span></span>

* <span data-ttu-id="c5a65-1273">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1273">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1274">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1274">Role</span></span>

* <span data-ttu-id="c5a65-1275">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1275">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="c5a65-1276">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1276">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="c5a65-1277">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1277">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1278">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1278">SQL</span></span>

* <span data-ttu-id="c5a65-1279">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1279">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="c5a65-1280">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1280">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1281">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1281">VM</span></span>

* <span data-ttu-id="c5a65-1282">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1282">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="c5a65-1283">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1283">November 14, 2017</span></span>

<span data-ttu-id="c5a65-1284">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="c5a65-1284">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-1285">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1285">ACR</span></span>

* <span data-ttu-id="c5a65-1286">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="c5a65-1286">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="c5a65-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1287">ACS</span></span>

* <span data-ttu-id="c5a65-1288">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1288">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="c5a65-1289">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1289">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="c5a65-1290">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1290">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="c5a65-1291">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-1291">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="c5a65-1292">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c5a65-1292">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1293">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1293">Appservice</span></span>

* <span data-ttu-id="c5a65-1294">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="c5a65-1294">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="c5a65-1295">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1295">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="c5a65-1296">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1296">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="c5a65-1297">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1297">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="c5a65-1298">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="c5a65-1298">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="c5a65-1299">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1299">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-1300">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1300">Batch</span></span>

* <span data-ttu-id="c5a65-1301">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1301">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="c5a65-1302">Batchai</span><span class="sxs-lookup"><span data-stu-id="c5a65-1302">Batchai</span></span>

* <span data-ttu-id="c5a65-1303">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1303">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="c5a65-1304">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1304">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="c5a65-1305">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1305">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="c5a65-1306">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1306">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="c5a65-1307">Cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-1307">Cloud</span></span>

* <span data-ttu-id="c5a65-1308">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="c5a65-1308">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1309">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1309">Container</span></span>

* <span data-ttu-id="c5a65-1310">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="c5a65-1310">Added support to open multiple ports</span></span>
* <span data-ttu-id="c5a65-1311">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1311">Added container group restart policy</span></span>
* <span data-ttu-id="c5a65-1312">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="c5a65-1312">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="c5a65-1313">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="c5a65-1313">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c5a65-1314">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c5a65-1314">Data Lake Analytics</span></span>

* <span data-ttu-id="c5a65-1315">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c5a65-1315">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c5a65-1316">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1316">Data Lake Store</span></span>

* <span data-ttu-id="c5a65-1317">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c5a65-1317">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-1318">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-1318">Extension</span></span>

* <span data-ttu-id="c5a65-1319">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="c5a65-1319">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="c5a65-1320">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="c5a65-1320">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-1321">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1321">IoT</span></span>

* <span data-ttu-id="c5a65-1322">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1322">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1323">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1323">Monitor</span></span>

* <span data-ttu-id="c5a65-1324">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1324">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1325">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1325">Network</span></span>

* <span data-ttu-id="c5a65-1326">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="c5a65-1326">Added support for CAA DNS records</span></span>
* <span data-ttu-id="c5a65-1327">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1327">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="c5a65-1328">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c5a65-1328">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="c5a65-1329">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1329">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="c5a65-1330">Réservations</span><span class="sxs-lookup"><span data-stu-id="c5a65-1330">Reservations</span></span>

* <span data-ttu-id="c5a65-1331">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1331">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1332">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1332">Resource</span></span>

* <span data-ttu-id="c5a65-1333">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c5a65-1333">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1334">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1334">SQL</span></span>

* <span data-ttu-id="c5a65-1335">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1335">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1336">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1336">Storage</span></span>

* <span data-ttu-id="c5a65-1337">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1337">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="c5a65-1338">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="c5a65-1338">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="c5a65-1339">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1339">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="c5a65-1340">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1340">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="c5a65-1341">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1341">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="c5a65-1342">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1342">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="c5a65-1343">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1343">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1344">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1344">VM</span></span>

* <span data-ttu-id="c5a65-1345">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1345">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="c5a65-1346">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1346">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="c5a65-1347">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="c5a65-1347">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="c5a65-1348">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1348">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="c5a65-1349">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1349">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c5a65-1350">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1350">October 24, 2017</span></span>

<span data-ttu-id="c5a65-1351">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c5a65-1351">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1352">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1352">Core</span></span>

* <span data-ttu-id="c5a65-1353">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1353">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-1354">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1354">ACR</span></span>

* <span data-ttu-id="c5a65-1355">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1355">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c5a65-1356">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="c5a65-1356">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c5a65-1357">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="c5a65-1357">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1358">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1358">ACS</span></span>

* <span data-ttu-id="c5a65-1359">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1359">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c5a65-1360">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1360">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1361">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1361">Appservice</span></span>

* <span data-ttu-id="c5a65-1362">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="c5a65-1362">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c5a65-1363">Composant</span><span class="sxs-lookup"><span data-stu-id="c5a65-1363">Component</span></span>

* <span data-ttu-id="c5a65-1364">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1364">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1365">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1365">Monitor</span></span>

* <span data-ttu-id="c5a65-1366">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1366">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1367">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1367">Resource</span></span>

* <span data-ttu-id="c5a65-1368">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1368">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c5a65-1369">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1369">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1370">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1370">VM</span></span>

* <span data-ttu-id="c5a65-1371">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1371">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c5a65-1372">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1372">October 9, 2017</span></span>

<span data-ttu-id="c5a65-1373">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c5a65-1373">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1374">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1374">Core</span></span>

* <span data-ttu-id="c5a65-1375">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c5a65-1375">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1376">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1376">Appservice</span></span>

* <span data-ttu-id="c5a65-1377">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1377">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-1378">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1378">Batch</span></span>

* <span data-ttu-id="c5a65-1379">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c5a65-1379">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c5a65-1380">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="c5a65-1380">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c5a65-1381">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1381">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c5a65-1382">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="c5a65-1382">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c5a65-1383">Batchai</span><span class="sxs-lookup"><span data-stu-id="c5a65-1383">Batchai</span></span>

* <span data-ttu-id="c5a65-1384">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="c5a65-1384">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-1385">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-1385">Keyvault</span></span>

* <span data-ttu-id="c5a65-1386">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1386">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c5a65-1387">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1387">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c5a65-1388">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1388">Network</span></span>

* <span data-ttu-id="c5a65-1389">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="c5a65-1389">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c5a65-1390">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1390">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1391">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1391">Resource</span></span>

* <span data-ttu-id="c5a65-1392">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1392">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c5a65-1393">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1393">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c5a65-1394">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1394">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c5a65-1395">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c5a65-1395">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1396">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1396">Sql</span></span>

* <span data-ttu-id="c5a65-1397">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="c5a65-1397">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c5a65-1398">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1398">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c5a65-1399">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="c5a65-1399">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1400">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1400">Storage</span></span>

* <span data-ttu-id="c5a65-1401">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="c5a65-1401">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1402">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1402">Vm</span></span>

* <span data-ttu-id="c5a65-1403">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1403">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c5a65-1404">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1404">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c5a65-1405">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1405">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c5a65-1406">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1406">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c5a65-1407">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1407">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c5a65-1408">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1408">September 22, 2017</span></span>

<span data-ttu-id="c5a65-1409">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c5a65-1409">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1410">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1410">Resource</span></span>

* <span data-ttu-id="c5a65-1411">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1411">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c5a65-1412">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="c5a65-1412">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c5a65-1413">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1413">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c5a65-1414">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1414">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1415">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1415">Network</span></span>

* <span data-ttu-id="c5a65-1416">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1416">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c5a65-1417">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1417">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c5a65-1418">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1418">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c5a65-1419">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1419">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c5a65-1420">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1420">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c5a65-1421">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1421">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c5a65-1422">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1422">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1423">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1423">Storage</span></span>

* <span data-ttu-id="c5a65-1424">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1424">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c5a65-1425">Événement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1425">Eventgrid</span></span>

* <span data-ttu-id="c5a65-1426">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1426">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1427">SQL</span></span>

* <span data-ttu-id="c5a65-1428">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1428">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c5a65-1429">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1429">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c5a65-1430">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1430">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-1431">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-1431">Keyvault</span></span>

* <span data-ttu-id="c5a65-1432">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="c5a65-1432">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1433">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1433">VM</span></span>

* <span data-ttu-id="c5a65-1434">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1434">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c5a65-1435">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="c5a65-1435">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c5a65-1436">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1436">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c5a65-1437">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1437">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c5a65-1438">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1438">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c5a65-1439">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1439">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1440">ACS</span></span>

* <span data-ttu-id="c5a65-1441">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="c5a65-1441">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1442">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1442">Appservice</span></span>

* <span data-ttu-id="c5a65-1443">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1443">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c5a65-1444">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c5a65-1444">Backup</span></span>

* <span data-ttu-id="c5a65-1445">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1445">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c5a65-1446">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1446">September 11, 2017</span></span>

<span data-ttu-id="c5a65-1447">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c5a65-1447">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c5a65-1448">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1448">Core</span></span>

* <span data-ttu-id="c5a65-1449">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="c5a65-1449">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c5a65-1450">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="c5a65-1450">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1451">Acs</span><span class="sxs-lookup"><span data-stu-id="c5a65-1451">Acs</span></span>

* <span data-ttu-id="c5a65-1452">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1452">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c5a65-1453">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="c5a65-1453">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1454">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1454">Appservice</span></span>

* <span data-ttu-id="c5a65-1455">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1455">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c5a65-1456">CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1456">CDN</span></span>

* <span data-ttu-id="c5a65-1457">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1457">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="c5a65-1458">Extension</span><span class="sxs-lookup"><span data-stu-id="c5a65-1458">Extension</span></span>

* <span data-ttu-id="c5a65-1459">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1459">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-1460">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-1460">Keyvault</span></span>

* <span data-ttu-id="c5a65-1461">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1461">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1462">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1462">Network</span></span>

* <span data-ttu-id="c5a65-1463">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1463">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c5a65-1464">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1464">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c5a65-1465">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1465">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c5a65-1466">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1466">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c5a65-1467">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1467">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1468">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1468">Resource</span></span>

* <span data-ttu-id="c5a65-1469">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1469">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c5a65-1470">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1470">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c5a65-1471">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="c5a65-1471">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c5a65-1472">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="c5a65-1472">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1473">SQL</span></span>

* <span data-ttu-id="c5a65-1474">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1474">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1475">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1475">VM</span></span>

* <span data-ttu-id="c5a65-1476">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="c5a65-1476">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c5a65-1477">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="c5a65-1477">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c5a65-1478">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1478">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c5a65-1479">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="c5a65-1479">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c5a65-1480">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="c5a65-1480">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c5a65-1481">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1481">August 31, 2017</span></span>

<span data-ttu-id="c5a65-1482">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c5a65-1482">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-1483">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-1483">Keyvault</span></span>

* <span data-ttu-id="c5a65-1484">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1484">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c5a65-1485">Sf</span><span class="sxs-lookup"><span data-stu-id="c5a65-1485">Sf</span></span>

* <span data-ttu-id="c5a65-1486">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1486">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1487">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1487">Storage</span></span>

* <span data-ttu-id="c5a65-1488">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="c5a65-1488">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c5a65-1489">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1489">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c5a65-1490">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1490">August 28, 2017</span></span>

<span data-ttu-id="c5a65-1491">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c5a65-1491">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c5a65-1492">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-1492">CLI</span></span>

* <span data-ttu-id="c5a65-1493">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1493">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1494">ACS</span></span>

* <span data-ttu-id="c5a65-1495">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c5a65-1495">Corrected preview regions</span></span>
* <span data-ttu-id="c5a65-1496">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1496">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="c5a65-1497">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1497">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1498">Appservice</span></span>

* <span data-ttu-id="c5a65-1499">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1499">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c5a65-1500">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1500">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c5a65-1501">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1501">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c5a65-1502">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1502">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c5a65-1503">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1503">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-1504">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1504">IoT</span></span>

* <span data-ttu-id="c5a65-1505">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1505">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1506">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1506">Network</span></span>

* <span data-ttu-id="c5a65-1507">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1507">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c5a65-1508">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1508">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c5a65-1509">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1509">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c5a65-1510">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1510">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c5a65-1511">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1511">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1512">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1512">Profile</span></span>

* <span data-ttu-id="c5a65-1513">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1513">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c5a65-1514">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c5a65-1514">Service Fabric</span></span>

* <span data-ttu-id="c5a65-1515">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1515">Preview release</span></span>
* <span data-ttu-id="c5a65-1516">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-1516">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c5a65-1517">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="c5a65-1517">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c5a65-1518">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1518">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1519">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1519">Storage</span></span>

* <span data-ttu-id="c5a65-1520">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="c5a65-1520">Enabled setting blob tier</span></span>
* <span data-ttu-id="c5a65-1521">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="c5a65-1521">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c5a65-1522">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1522">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="c5a65-1523">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="c5a65-1523">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c5a65-1524">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1524">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c5a65-1525">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1525">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1526">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1526">VM</span></span>

* <span data-ttu-id="c5a65-1527">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1527">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c5a65-1528">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c5a65-1528">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="c5a65-1529">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1529">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="c5a65-1530">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="c5a65-1530">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c5a65-1531">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="c5a65-1531">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c5a65-1532">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1532">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c5a65-1533">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1533">August 15, 2017</span></span>

<span data-ttu-id="c5a65-1534">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c5a65-1534">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1535">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1535">ACS</span></span>

* <span data-ttu-id="c5a65-1536">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1536">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1537">Appservice</span></span>

* <span data-ttu-id="c5a65-1538">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="c5a65-1538">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c5a65-1539">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c5a65-1539">Event Grid</span></span>

* <span data-ttu-id="c5a65-1540">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1540">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c5a65-1541">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1541">August 11, 2017</span></span>

<span data-ttu-id="c5a65-1542">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c5a65-1542">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1543">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1543">ACS</span></span>

* <span data-ttu-id="c5a65-1544">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c5a65-1544">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-1545">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1545">Batch</span></span>

* <span data-ttu-id="c5a65-1546">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c5a65-1546">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c5a65-1547">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-1547">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c5a65-1548">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="c5a65-1548">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c5a65-1549">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1549">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c5a65-1550">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="c5a65-1550">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c5a65-1551">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="c5a65-1551">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c5a65-1552">Composant</span><span class="sxs-lookup"><span data-stu-id="c5a65-1552">Component</span></span>

* <span data-ttu-id="c5a65-1553">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1553">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c5a65-1554">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1554">Container</span></span>

* <span data-ttu-id="c5a65-1555">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1555">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c5a65-1556">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1556">Data Lake Store</span></span>

* <span data-ttu-id="c5a65-1557">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="c5a65-1557">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c5a65-1558">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c5a65-1558">Event Grid</span></span>

* <span data-ttu-id="c5a65-1559">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c5a65-1559">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1560">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1560">Network</span></span>

* <span data-ttu-id="c5a65-1561">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="c5a65-1561">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c5a65-1562">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1562">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c5a65-1563">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="c5a65-1563">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c5a65-1564">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1564">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1565">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1565">Profile</span></span>

* <span data-ttu-id="c5a65-1566">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1566">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1567">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1567">Storage</span></span>

* <span data-ttu-id="c5a65-1568">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c5a65-1568">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1569">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1569">VM</span></span>

* <span data-ttu-id="c5a65-1570">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="c5a65-1570">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c5a65-1571">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1571">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c5a65-1572">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1572">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c5a65-1573">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="c5a65-1573">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c5a65-1574">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1574">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c5a65-1575">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1575">July 28, 2017</span></span>

<span data-ttu-id="c5a65-1576">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c5a65-1576">Version 2.0.12</span></span>

* <span data-ttu-id="c5a65-1577">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1577">Added container commands</span></span>
* <span data-ttu-id="c5a65-1578">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="c5a65-1578">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c5a65-1579">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1579">Core</span></span>

* <span data-ttu-id="c5a65-1580">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="c5a65-1580">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c5a65-1581">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1581">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c5a65-1582">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1582">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c5a65-1583">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1583">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c5a65-1584">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="c5a65-1584">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c5a65-1585">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1585">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c5a65-1586">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1586">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c5a65-1587">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1587">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c5a65-1588">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1588">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c5a65-1589">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1589">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c5a65-1590">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="c5a65-1590">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c5a65-1591">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1591">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c5a65-1592">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c5a65-1592">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c5a65-1593">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c5a65-1593">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c5a65-1594">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c5a65-1594">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c5a65-1595">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1595">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c5a65-1596">ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1596">ACR</span></span>

* <span data-ttu-id="c5a65-1597">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1597">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c5a65-1598">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1598">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c5a65-1599">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1599">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c5a65-1600">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="c5a65-1600">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c5a65-1601">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="c5a65-1601">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c5a65-1602">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="c5a65-1602">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1603">ACS</span></span>

* <span data-ttu-id="c5a65-1604">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c5a65-1604">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1605">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1605">Appservice</span></span>

* <span data-ttu-id="c5a65-1606">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="c5a65-1606">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c5a65-1607">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1607">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c5a65-1608">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1608">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c5a65-1609">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1609">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c5a65-1610">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1610">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c5a65-1611">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1611">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c5a65-1612">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1612">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c5a65-1613">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1613">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c5a65-1614">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1614">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c5a65-1615">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1615">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c5a65-1616">Batch</span><span class="sxs-lookup"><span data-stu-id="c5a65-1616">Batch</span></span>

* <span data-ttu-id="c5a65-1617">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="c5a65-1617">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c5a65-1618">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1618">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c5a65-1619">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1619">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c5a65-1620">CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1620">CDN</span></span>

* <span data-ttu-id="c5a65-1621">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c5a65-1621">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="c5a65-1622">Cloud</span><span class="sxs-lookup"><span data-stu-id="c5a65-1622">Cloud</span></span>

* <span data-ttu-id="c5a65-1623">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="c5a65-1623">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c5a65-1624">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1624">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c5a65-1625">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="c5a65-1625">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c5a65-1626">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="c5a65-1626">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c5a65-1627">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1627">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c5a65-1628">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-1628">CosmosDB</span></span>

* <span data-ttu-id="c5a65-1629">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1629">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c5a65-1630">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="c5a65-1630">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c5a65-1631">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c5a65-1631">Data Lake Analytics</span></span>

* <span data-ttu-id="c5a65-1632">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1632">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c5a65-1633">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1633">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c5a65-1634">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1634">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c5a65-1635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1635">Data Lake Store</span></span>

* <span data-ttu-id="c5a65-1636">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1636">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c5a65-1637">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="c5a65-1637">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c5a65-1638">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1638">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c5a65-1639">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1639">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c5a65-1640">Interactive</span><span class="sxs-lookup"><span data-stu-id="c5a65-1640">Interactive</span></span>

* <span data-ttu-id="c5a65-1641">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="c5a65-1641">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c5a65-1642">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="c5a65-1642">Increased test coverage</span></span>
* <span data-ttu-id="c5a65-1643">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="c5a65-1643">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c5a65-1644">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1644">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c5a65-1645">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1645">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c5a65-1646">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1646">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c5a65-1647">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1647">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c5a65-1648">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1648">Added `--progress` flag</span></span>
* <span data-ttu-id="c5a65-1649">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="c5a65-1649">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c5a65-1650">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1650">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c5a65-1651">IoT</span><span class="sxs-lookup"><span data-stu-id="c5a65-1651">IoT</span></span>

* <span data-ttu-id="c5a65-1652">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1652">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c5a65-1653">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1653">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c5a65-1654">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1654">Key vault</span></span>

* <span data-ttu-id="c5a65-1655">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1655">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c5a65-1656">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1656">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c5a65-1657">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1657">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c5a65-1658">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1658">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c5a65-1659">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1659">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c5a65-1660">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1660">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c5a65-1661">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1661">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c5a65-1662">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1662">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c5a65-1663">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1663">Lab</span></span>

* <span data-ttu-id="c5a65-1664">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1664">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c5a65-1665">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1665">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1666">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1666">Monitor</span></span>

* <span data-ttu-id="c5a65-1667">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1667">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c5a65-1668">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1668">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c5a65-1669">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1669">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c5a65-1670">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1670">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c5a65-1671">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1671">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c5a65-1672">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c5a65-1672">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c5a65-1673">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="c5a65-1673">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c5a65-1674">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1674">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c5a65-1675">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1675">`location` no longer required</span></span>
  * <span data-ttu-id="c5a65-1676">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="c5a65-1676">Add name and ID support for target</span></span>
  * <span data-ttu-id="c5a65-1677">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1677">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c5a65-1678">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1678">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c5a65-1679">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="c5a65-1679">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c5a65-1680">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="c5a65-1680">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c5a65-1681">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1681">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c5a65-1682">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1682">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1683">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1683">Network</span></span>

* <span data-ttu-id="c5a65-1684">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1684">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c5a65-1685">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1685">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c5a65-1686">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="c5a65-1686">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c5a65-1687">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="c5a65-1687">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c5a65-1688">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1688">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c5a65-1689">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1689">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c5a65-1690">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1690">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c5a65-1691">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1691">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c5a65-1692">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1692">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c5a65-1693">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1693">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c5a65-1694">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1694">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c5a65-1695">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1695">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c5a65-1696">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1696">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c5a65-1697">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1697">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c5a65-1698">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1698">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c5a65-1699">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1699">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c5a65-1700">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1700">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c5a65-1701">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1701">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c5a65-1702">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1702">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c5a65-1703">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1703">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c5a65-1704">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1704">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c5a65-1705">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1705">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c5a65-1706">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1706">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c5a65-1707">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c5a65-1707">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c5a65-1708">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c5a65-1708">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c5a65-1709">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c5a65-1709">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c5a65-1710">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c5a65-1710">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1711">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1711">Profile</span></span>

* <span data-ttu-id="c5a65-1712">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1712">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c5a65-1713">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1713">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c5a65-1714">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="c5a65-1714">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c5a65-1715">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1715">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c5a65-1716">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="c5a65-1716">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c5a65-1717">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c5a65-1717">RDBMS</span></span>

* <span data-ttu-id="c5a65-1718">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1718">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c5a65-1719">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1719">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c5a65-1720">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1720">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c5a65-1721">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1721">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1722">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1722">Resource</span></span>

* <span data-ttu-id="c5a65-1723">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1723">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c5a65-1724">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1724">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c5a65-1725">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1725">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c5a65-1726">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="c5a65-1726">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c5a65-1727">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1727">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c5a65-1728">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1728">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c5a65-1729">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1729">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c5a65-1730">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c5a65-1730">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1731">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1731">Role</span></span>

* <span data-ttu-id="c5a65-1732">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1732">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c5a65-1733">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1733">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c5a65-1734">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="c5a65-1734">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c5a65-1735">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1735">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c5a65-1736">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1736">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c5a65-1737">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c5a65-1737">Service Fabric</span></span>
* <span data-ttu-id="c5a65-1738">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1738">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c5a65-1739">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1739">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c5a65-1740">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1740">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1741">SQL</span></span>

* <span data-ttu-id="c5a65-1742">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1742">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c5a65-1743">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1743">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c5a65-1744">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1744">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1745">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1745">Storage</span></span>

* <span data-ttu-id="c5a65-1746">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1746">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c5a65-1747">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="c5a65-1747">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c5a65-1748">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1748">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c5a65-1749">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1749">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="c5a65-1750">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1750">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="c5a65-1751">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1751">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1752">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1752">VM</span></span>

* <span data-ttu-id="c5a65-1753">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1753">Support configuring nsg</span></span>
* <span data-ttu-id="c5a65-1754">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1754">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c5a65-1755">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="c5a65-1755">Support managed service identities</span></span>
* <span data-ttu-id="c5a65-1756">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1756">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="c5a65-1757">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="c5a65-1757">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c5a65-1758">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1758">May 10, 2017</span></span>

<span data-ttu-id="c5a65-1759">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c5a65-1759">Version 2.0.6</span></span>

* <span data-ttu-id="c5a65-1760">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c5a65-1760">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c5a65-1761">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1761">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c5a65-1762">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1762">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="c5a65-1763">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c5a65-1763">Include Cognitive Services module</span></span>
* <span data-ttu-id="c5a65-1764">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c5a65-1764">Include Service Fabric module</span></span>
* <span data-ttu-id="c5a65-1765">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1765">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="c5a65-1766">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1766">Add support for CDN commands</span></span>
* <span data-ttu-id="c5a65-1767">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="c5a65-1767">Remove Container module</span></span>
* <span data-ttu-id="c5a65-1768">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1768">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c5a65-1769">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1769">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c5a65-1770">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1770">Core</span></span>

* <span data-ttu-id="c5a65-1771">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1771">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="c5a65-1772">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1772">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c5a65-1773">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1773">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c5a65-1774">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1774">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c5a65-1775">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1775">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c5a65-1776">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1776">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c5a65-1777">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1777">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c5a65-1778">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1778">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c5a65-1779">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1779">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c5a65-1780">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="c5a65-1780">core: Improved performance</span></span>
* <span data-ttu-id="c5a65-1781">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c5a65-1781">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c5a65-1782">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="c5a65-1782">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1783">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1783">ACS</span></span>

* <span data-ttu-id="c5a65-1784">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c5a65-1784">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c5a65-1785">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="c5a65-1785">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c5a65-1786">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="c5a65-1786">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c5a65-1787">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1787">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1788">AppService</span></span>

* <span data-ttu-id="c5a65-1789">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1789">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c5a65-1790">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1790">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c5a65-1791">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1791">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c5a65-1792">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="c5a65-1792">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c5a65-1793">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1793">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c5a65-1794">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1794">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c5a65-1795">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="c5a65-1795">support slot swap with preview</span></span>
* <span data-ttu-id="c5a65-1796">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1796">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c5a65-1797">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1797">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c5a65-1798">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-1798">CosmosDB</span></span>

* <span data-ttu-id="c5a65-1799">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c5a65-1799">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="c5a65-1800">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="c5a65-1800">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c5a65-1801">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="c5a65-1801">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c5a65-1802">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c5a65-1802">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c5a65-1803">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c5a65-1803">Data Lake Analytics</span></span>

* <span data-ttu-id="c5a65-1804">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1804">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="c5a65-1805">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1805">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c5a65-1806">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1806">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c5a65-1807">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1807">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c5a65-1808">Table</span><span class="sxs-lookup"><span data-stu-id="c5a65-1808">Table</span></span>
  * <span data-ttu-id="c5a65-1809">Fonction table</span><span class="sxs-lookup"><span data-stu-id="c5a65-1809">Table valued function</span></span>
  * <span data-ttu-id="c5a65-1810">Affichage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1810">View</span></span>
  * <span data-ttu-id="c5a65-1811">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1811">Table Statistics.</span></span> <span data-ttu-id="c5a65-1812">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="c5a65-1812">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c5a65-1813">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1813">Data Lake Store</span></span>

* <span data-ttu-id="c5a65-1814">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="c5a65-1814">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="c5a65-1815">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1815">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c5a65-1816">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1816">missed help for access show.</span></span> <span data-ttu-id="c5a65-1817">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1817">adding it.</span></span> <span data-ttu-id="c5a65-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c5a65-1819">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c5a65-1819">Find</span></span>

* <span data-ttu-id="c5a65-1820">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="c5a65-1820">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c5a65-1821">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5a65-1821">KeyVault</span></span>

* <span data-ttu-id="c5a65-1822">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="c5a65-1822">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c5a65-1823">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c5a65-1823">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="c5a65-1824">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="c5a65-1824">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c5a65-1825">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="c5a65-1825">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="c5a65-1826">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1826">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c5a65-1827">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1827">Lab</span></span>

* <span data-ttu-id="c5a65-1828">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1828">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="c5a65-1829">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1829">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="c5a65-1830">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1830">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="c5a65-1831">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1831">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="c5a65-1832">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="c5a65-1832">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="c5a65-1833">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c5a65-1833">Monitor</span></span>

* <span data-ttu-id="c5a65-1834">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1834">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c5a65-1835">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1835">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c5a65-1836">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1836">Network</span></span>

* <span data-ttu-id="c5a65-1837">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1837">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="c5a65-1838">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1838">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="c5a65-1839">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c5a65-1839">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="c5a65-1840">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c5a65-1840">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="c5a65-1841">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="c5a65-1841">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="c5a65-1842">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c5a65-1842">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="c5a65-1843">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1843">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="c5a65-1844">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c5a65-1844">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="c5a65-1845">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1845">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="c5a65-1846">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1846">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c5a65-1847">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1847">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="c5a65-1848">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1848">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="c5a65-1849">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1849">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="c5a65-1850">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="c5a65-1850">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="c5a65-1851">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c5a65-1851">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="c5a65-1852">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="c5a65-1852">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="c5a65-1853">Profil</span><span class="sxs-lookup"><span data-stu-id="c5a65-1853">Profile</span></span>

* <span data-ttu-id="c5a65-1854">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1854">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c5a65-1855">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1855">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c5a65-1856">Redis</span><span class="sxs-lookup"><span data-stu-id="c5a65-1856">Redis</span></span>

* <span data-ttu-id="c5a65-1857">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="c5a65-1857">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c5a65-1858">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="c5a65-1858">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="c5a65-1859">Ressource</span><span class="sxs-lookup"><span data-stu-id="c5a65-1859">Resource</span></span>

* <span data-ttu-id="c5a65-1860">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1860">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c5a65-1861">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1861">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c5a65-1862">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1862">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c5a65-1863">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1863">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c5a65-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c5a65-1865">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1865">Add docs for az lock update.</span></span> <span data-ttu-id="c5a65-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c5a65-1867">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1867">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c5a65-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c5a65-1869">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1869">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c5a65-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c5a65-1871">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1871">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c5a65-1872">Rôle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1872">Role</span></span>

* <span data-ttu-id="c5a65-1873">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1873">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c5a65-1874">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1874">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c5a65-1875">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1875">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c5a65-1876">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="c5a65-1876">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c5a65-1877">SQL</span><span class="sxs-lookup"><span data-stu-id="c5a65-1877">SQL</span></span>

* <span data-ttu-id="c5a65-1878">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="c5a65-1878">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="c5a65-1879">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1879">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c5a65-1880">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1880">Storage</span></span>

* <span data-ttu-id="c5a65-1881">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="c5a65-1881">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="c5a65-1882">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c5a65-1882">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c5a65-1883">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="c5a65-1883">Add support for large block blob upload</span></span>
* <span data-ttu-id="c5a65-1884">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="c5a65-1884">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1885">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1885">VM</span></span>

* <span data-ttu-id="c5a65-1886">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="c5a65-1886">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c5a65-1887">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1887">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c5a65-1888">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c5a65-1888">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c5a65-1889">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c5a65-1889">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c5a65-1890">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="c5a65-1890">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c5a65-1891">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="c5a65-1891">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c5a65-1892">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1892">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c5a65-1893">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1893">April 3, 2017</span></span>

<span data-ttu-id="c5a65-1894">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c5a65-1894">Version 2.0.2</span></span>

<span data-ttu-id="c5a65-1895">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="c5a65-1895">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="c5a65-1896">Principal</span><span class="sxs-lookup"><span data-stu-id="c5a65-1896">Core</span></span>

* <span data-ttu-id="c5a65-1897">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1897">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="c5a65-1898">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1898">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c5a65-1899">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1899">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c5a65-1900">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1900">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c5a65-1901">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1901">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c5a65-1902">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1902">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c5a65-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c5a65-1904">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="c5a65-1904">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c5a65-1905">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="c5a65-1905">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="c5a65-1906">ACS</span><span class="sxs-lookup"><span data-stu-id="c5a65-1906">ACS</span></span>

* <span data-ttu-id="c5a65-1907">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1907">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c5a65-1908">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1908">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c5a65-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c5a65-1910">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1910">Add support for windows clusters.</span></span> <span data-ttu-id="c5a65-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c5a65-1912">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1912">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c5a65-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="c5a65-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="c5a65-1914">AppService</span></span>

* <span data-ttu-id="c5a65-1915">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1915">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c5a65-1916">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1916">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c5a65-1917">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1917">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c5a65-1918">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1918">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="c5a65-1919">DataLake</span><span class="sxs-lookup"><span data-stu-id="c5a65-1919">DataLake</span></span>

* <span data-ttu-id="c5a65-1920">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c5a65-1920">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="c5a65-1921">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c5a65-1921">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="c5a65-1922">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c5a65-1922">DocuemntDB</span></span>

* <span data-ttu-id="c5a65-1923">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1923">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c5a65-1924">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c5a65-1924">VM</span></span>

* <span data-ttu-id="c5a65-1925">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1925">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c5a65-1926">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1926">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c5a65-1927">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1927">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c5a65-1928">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1928">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c5a65-1929">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1929">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c5a65-1930">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1930">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="c5a65-1931">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c5a65-1931">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c5a65-1932">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="c5a65-1932">February 27, 2017</span></span>

<span data-ttu-id="c5a65-1933">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c5a65-1933">Version 2.0.0</span></span>

<span data-ttu-id="c5a65-1934">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1934">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="c5a65-1935">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1935">Container Service (acs)</span></span>
- <span data-ttu-id="c5a65-1936">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1936">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c5a65-1937">Réseau</span><span class="sxs-lookup"><span data-stu-id="c5a65-1937">Networking</span></span>
- <span data-ttu-id="c5a65-1938">Stockage</span><span class="sxs-lookup"><span data-stu-id="c5a65-1938">Storage</span></span>

<span data-ttu-id="c5a65-1939">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1939">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="c5a65-1940">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1940">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="c5a65-1941">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1941">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="c5a65-1942">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1942">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="c5a65-1943">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c5a65-1943">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="c5a65-1944">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="c5a65-1944">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c5a65-1945">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c5a65-1945">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c5a65-1946">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c5a65-1946">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="c5a65-1947">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c5a65-1947">Provide feedback from the command line with the `az feedback` command</span></span>

