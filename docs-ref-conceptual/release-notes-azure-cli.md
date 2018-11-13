---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 51b8b8cad6d25f916006b8e68b8f300587f5d45b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222563"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="d5cd3-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-103">Azure CLI release notes</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="d5cd3-104">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-104">November 6, 2018</span></span>

<span data-ttu-id="d5cd3-105">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="d5cd3-105">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-106">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-106">Core</span></span>
* <span data-ttu-id="d5cd3-107">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="d5cd3-107">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-108">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-108">ACR</span></span>
* <span data-ttu-id="d5cd3-109">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="d5cd3-109">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="d5cd3-110">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="d5cd3-110">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-111">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-111">ACS</span></span>
* <span data-ttu-id="d5cd3-112">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-112">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="d5cd3-113">Advisor</span><span class="sxs-lookup"><span data-stu-id="d5cd3-113">Advisor</span></span>
* <span data-ttu-id="d5cd3-114">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-114">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="d5cd3-115">AMS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-115">AMS</span></span>
* <span data-ttu-id="d5cd3-116">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-116">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="d5cd3-117">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-117">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="d5cd3-118">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-118">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="d5cd3-119">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="d5cd3-119">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="d5cd3-120">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-120">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="d5cd3-121">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-121">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="d5cd3-122">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-122">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="d5cd3-123">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-123">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="d5cd3-124">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-124">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="d5cd3-125">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-125">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="d5cd3-126">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-126">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="d5cd3-127">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-127">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="d5cd3-128">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="d5cd3-128">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="d5cd3-129">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-129">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="d5cd3-130">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-130">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="d5cd3-131">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="d5cd3-131">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="d5cd3-132">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-132">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-133">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-133">AppService</span></span>
* <span data-ttu-id="d5cd3-134">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-134">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="d5cd3-135">Configuration</span><span class="sxs-lookup"><span data-stu-id="d5cd3-135">Configure</span></span>
* <span data-ttu-id="d5cd3-136">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-136">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-137">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-137">Container</span></span>
* <span data-ttu-id="d5cd3-138">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="d5cd3-138">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="d5cd3-139">Event Hub</span><span class="sxs-lookup"><span data-stu-id="d5cd3-139">EventHub</span></span>
* <span data-ttu-id="d5cd3-140">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-140">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-141">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-141">Interactive</span></span>
* <span data-ttu-id="d5cd3-142">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="d5cd3-142">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-143">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-143">Monitor</span></span>
* <span data-ttu-id="d5cd3-144">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-144">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-145">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-145">Network</span></span>
* <span data-ttu-id="d5cd3-146">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-146">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="d5cd3-147">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-147">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="d5cd3-148">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-148">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="d5cd3-149">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-149">Profile</span></span>
* <span data-ttu-id="d5cd3-150">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-150">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-151">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-151">RDBMS</span></span>
* <span data-ttu-id="d5cd3-152">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="d5cd3-152">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-153">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-153">Resource</span></span>
* <span data-ttu-id="d5cd3-154">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-154">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-155">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-155">Role</span></span>
* <span data-ttu-id="d5cd3-156">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="d5cd3-156">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="d5cd3-157">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-157">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="d5cd3-158">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="d5cd3-158">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-159">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-159">Storage</span></span>
* <span data-ttu-id="d5cd3-160">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-160">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-161">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-161">VM</span></span>
* <span data-ttu-id="d5cd3-162">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-162">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="d5cd3-163">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-163">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="d5cd3-164">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="d5cd3-164">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="d5cd3-165">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="d5cd3-165">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="d5cd3-166">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="d5cd3-166">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="d5cd3-167">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-167">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="d5cd3-168">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-168">October 23, 2018</span></span>

<span data-ttu-id="d5cd3-169">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="d5cd3-169">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-170">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-170">Core</span></span>
* <span data-ttu-id="d5cd3-171">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-171">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="d5cd3-172">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-172">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-173">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-173">ACR</span></span>
* <span data-ttu-id="d5cd3-174">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="d5cd3-174">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="d5cd3-175">CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-175">CDN</span></span>
* <span data-ttu-id="d5cd3-176">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-176">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="d5cd3-177">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-177">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-178">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-178">Container</span></span>
* <span data-ttu-id="d5cd3-179">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="d5cd3-179">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="d5cd3-180">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-180">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="d5cd3-181">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="d5cd3-181">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="d5cd3-182">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-182">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="d5cd3-183">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="d5cd3-183">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="d5cd3-184">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="d5cd3-184">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="d5cd3-185">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-185">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d5cd3-186">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-186">CosmosDB</span></span>
* <span data-ttu-id="d5cd3-187">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-187">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-188">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-188">Interactive</span></span>
* <span data-ttu-id="d5cd3-189">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="d5cd3-189">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="d5cd3-190">IoT Central</span><span class="sxs-lookup"><span data-stu-id="d5cd3-190">IoT Central</span></span>
* <span data-ttu-id="d5cd3-191">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="d5cd3-191">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="d5cd3-192">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="d5cd3-192">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-193">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-193">Monitor</span></span>
* <span data-ttu-id="d5cd3-194">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-194">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="d5cd3-195">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-195">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="d5cd3-196">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="d5cd3-196">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d5cd3-197">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-197">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="d5cd3-198">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-198">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="d5cd3-199">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-199">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="d5cd3-200">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-200">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="d5cd3-201">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="d5cd3-201">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d5cd3-202">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-202">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="d5cd3-203">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-203">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-204">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-204">Network</span></span>
* <span data-ttu-id="d5cd3-205">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-205">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="d5cd3-206">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-206">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="d5cd3-207">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-207">ServiceBus</span></span>
* <span data-ttu-id="d5cd3-208">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-208">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-209">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-209">SQL</span></span>
* <span data-ttu-id="d5cd3-210">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-210">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-211">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-211">Storage</span></span>
* <span data-ttu-id="d5cd3-212">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="d5cd3-212">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="d5cd3-213">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-213">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-214">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-214">VM</span></span>
* <span data-ttu-id="d5cd3-215">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-215">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="d5cd3-216">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-216">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="d5cd3-217">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-217">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="d5cd3-218">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-218">October 16, 2018</span></span>

<span data-ttu-id="d5cd3-219">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="d5cd3-219">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-220">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-220">VM</span></span>
* <span data-ttu-id="d5cd3-221">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="d5cd3-221">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="d5cd3-222">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-222">October 9, 2018</span></span>

<span data-ttu-id="d5cd3-223">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="d5cd3-223">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-224">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-224">Core</span></span>
* <span data-ttu-id="d5cd3-225">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-225">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-226">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-226">ACR</span></span>
* <span data-ttu-id="d5cd3-227">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="d5cd3-227">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-228">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-228">ACS</span></span>
* <span data-ttu-id="d5cd3-229">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="d5cd3-229">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="d5cd3-230">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="d5cd3-230">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="d5cd3-231">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-231">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="d5cd3-232">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-232">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-233">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-233">Container</span></span>
* <span data-ttu-id="d5cd3-234">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-234">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="d5cd3-235">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-235">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="d5cd3-236">Event Hub</span><span class="sxs-lookup"><span data-stu-id="d5cd3-236">Event Hub</span></span>
* <span data-ttu-id="d5cd3-237">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-237">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="d5cd3-238">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-238">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="d5cd3-239">Extensions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-239">Extensions</span></span>
* <span data-ttu-id="d5cd3-240">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-240">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d5cd3-241">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d5cd3-241">HDInsight</span></span>
* <span data-ttu-id="d5cd3-242">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-242">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-243">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-243">IoT</span></span>
* <span data-ttu-id="d5cd3-244">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="d5cd3-244">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-245">KeyVault</span></span>
* <span data-ttu-id="d5cd3-246">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="d5cd3-246">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-247">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-247">Network</span></span>
* <span data-ttu-id="d5cd3-248">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-248">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="d5cd3-249">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="d5cd3-249">See #6052</span></span>
* <span data-ttu-id="d5cd3-250">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-250">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="d5cd3-251">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="d5cd3-251">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="d5cd3-252">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-252">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="d5cd3-253">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-253">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="d5cd3-254">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-254">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="d5cd3-255">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-255">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-256">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-256">Role</span></span>
* <span data-ttu-id="d5cd3-257">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-257">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="d5cd3-258">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-258">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="d5cd3-259">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="d5cd3-259">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="d5cd3-260">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-260">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="d5cd3-261">Service Bus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-261">Service Bus</span></span>
* <span data-ttu-id="d5cd3-262">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-262">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-263">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-263">VM</span></span>
* <span data-ttu-id="d5cd3-264">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-264">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="d5cd3-265">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-265">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="d5cd3-266">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-266">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="d5cd3-267">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-267">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="d5cd3-268">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-268">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="d5cd3-269">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-269">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="d5cd3-270">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-270">September 21, 2018</span></span>

<span data-ttu-id="d5cd3-271">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="d5cd3-271">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-272">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-272">ACR</span></span>
* <span data-ttu-id="d5cd3-273">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-273">Added ACR Task commands</span></span>
* <span data-ttu-id="d5cd3-274">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-274">Added quick run command</span></span>
* <span data-ttu-id="d5cd3-275">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-275">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="d5cd3-276">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-276">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="d5cd3-277">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-277">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="d5cd3-278">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="d5cd3-278">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-279">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-279">ACS</span></span>
* <span data-ttu-id="d5cd3-280">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-280">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="d5cd3-281">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="d5cd3-281">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-282">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-282">AppService</span></span>

* <span data-ttu-id="d5cd3-283">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-283">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="d5cd3-284">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="d5cd3-284">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="d5cd3-285">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="d5cd3-285">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="d5cd3-286">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-286">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-287">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-287">Batch</span></span>
* <span data-ttu-id="d5cd3-288">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="d5cd3-288">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="d5cd3-289">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-289">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="d5cd3-290">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-290">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="d5cd3-291">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-291">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d5cd3-292">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-292">Batch AI</span></span> 
* <span data-ttu-id="d5cd3-293">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-293">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d5cd3-294">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-294">Cognitive Services</span></span>
* <span data-ttu-id="d5cd3-295">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-295">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="d5cd3-296">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-296">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="d5cd3-297">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-297">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="d5cd3-298">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-298">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="d5cd3-299">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-299">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="d5cd3-300">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-300">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-301">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-301">Container</span></span>
* <span data-ttu-id="d5cd3-302">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="d5cd3-302">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="d5cd3-303">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-303">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="d5cd3-304">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-304">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="d5cd3-305">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-305">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="d5cd3-306">DataLake</span><span class="sxs-lookup"><span data-stu-id="d5cd3-306">Datalake</span></span>
* <span data-ttu-id="d5cd3-307">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-307">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="d5cd3-308">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-308">Interactive Shell</span></span>
* <span data-ttu-id="d5cd3-309">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-309">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="d5cd3-310">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-310">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-311">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-311">IoT</span></span>
* <span data-ttu-id="d5cd3-312">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-312">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="d5cd3-313">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-313">Key Vault</span></span>
* <span data-ttu-id="d5cd3-314">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="d5cd3-314">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-315">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-315">Network</span></span>
* <span data-ttu-id="d5cd3-316">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-316">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="d5cd3-317">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-317">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="d5cd3-318">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="d5cd3-318">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="d5cd3-319">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-319">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="d5cd3-320">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-320">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="d5cd3-321">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-321">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="d5cd3-322">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-322">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="d5cd3-323">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-323">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="d5cd3-324">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-324">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="d5cd3-325">`network express-route create/update` : ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-325">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="d5cd3-326">`network vnet subnet create/update` : ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-326">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="d5cd3-327">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-327">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="d5cd3-328">`network traffic-manager profile create/update` : ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-328">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="d5cd3-329">`network lb frontend-ip create/update` : correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-329">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="d5cd3-330">`dns record-set * create/update` : ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-330">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="d5cd3-331">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="d5cd3-331">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="d5cd3-332">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-332">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="d5cd3-333">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-333">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-334">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-334">RDBMS</span></span>
* <span data-ttu-id="d5cd3-335">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-335">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="d5cd3-336">Réservation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-336">Reservation</span></span>
* <span data-ttu-id="d5cd3-337">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-337">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="d5cd3-338">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-338">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="d5cd3-339">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="d5cd3-339">Manage App</span></span>
* <span data-ttu-id="d5cd3-340">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-340">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="d5cd3-341">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="d5cd3-341">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-342">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-342">Role</span></span>
* <span data-ttu-id="d5cd3-343">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-343">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="d5cd3-344">SignalR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-344">SignalR</span></span>
* <span data-ttu-id="d5cd3-345">Première version</span><span class="sxs-lookup"><span data-stu-id="d5cd3-345">First release</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-346">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-346">Storage</span></span>
* <span data-ttu-id="d5cd3-347">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="d5cd3-347">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="d5cd3-348">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="d5cd3-348">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-349">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-349">VM</span></span>
* <span data-ttu-id="d5cd3-350">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-350">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="d5cd3-351">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-351">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="d5cd3-352">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-352">August 28, 2018</span></span>

<span data-ttu-id="d5cd3-353">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="d5cd3-353">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-354">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-354">Core</span></span>

* <span data-ttu-id="d5cd3-355">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-355">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="d5cd3-356">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5cd3-356">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-357">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-357">ACR</span></span>

* <span data-ttu-id="d5cd3-358">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="d5cd3-358">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="d5cd3-359">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-359">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-360">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-360">ACS</span></span>

* <span data-ttu-id="d5cd3-361">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-361">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="d5cd3-362">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="d5cd3-362">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-363">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-363">AppService</span></span>

* <span data-ttu-id="d5cd3-364">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="d5cd3-364">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="d5cd3-365">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="d5cd3-365">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="d5cd3-366">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-366">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="d5cd3-367">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="d5cd3-367">Backup</span></span>

* <span data-ttu-id="d5cd3-368">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-368">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="d5cd3-369">Service de robot</span><span class="sxs-lookup"><span data-stu-id="d5cd3-369">Bot Service</span></span>

* <span data-ttu-id="d5cd3-370">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-370">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d5cd3-371">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-371">Cognitive Services</span></span>

* <span data-ttu-id="d5cd3-372">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-372">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-373">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-373">IoT</span></span>

* <span data-ttu-id="d5cd3-374">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-374">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-375">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-375">Monitor</span></span>

* <span data-ttu-id="d5cd3-376">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-376">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="d5cd3-377">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-377">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-378">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-378">Network</span></span>

* <span data-ttu-id="d5cd3-379">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-379">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-380">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-380">Resource</span></span>

* <span data-ttu-id="d5cd3-381">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-381">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-382">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-382">Storage</span></span>

* <span data-ttu-id="d5cd3-383">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-383">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-384">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-384">VM</span></span>

* <span data-ttu-id="d5cd3-385">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-385">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="d5cd3-386">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-386">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="d5cd3-387">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-387">Auguest 14, 2018</span></span>

<span data-ttu-id="d5cd3-388">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="d5cd3-388">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-389">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-389">Core</span></span>

* <span data-ttu-id="d5cd3-390">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-390">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="d5cd3-391">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="d5cd3-391">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="d5cd3-392">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-392">Telemetry</span></span>

* <span data-ttu-id="d5cd3-393">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-393">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-394">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-394">ACR</span></span>

* <span data-ttu-id="d5cd3-395">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-395">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="d5cd3-396">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-396">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-397">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-397">ACS</span></span>

* <span data-ttu-id="d5cd3-398">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-398">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="d5cd3-399">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-399">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="d5cd3-400">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-400">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="d5cd3-401">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-401">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="d5cd3-402">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="d5cd3-402">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="d5cd3-403">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-403">AppService</span></span>

* <span data-ttu-id="d5cd3-404">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-404">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="d5cd3-405">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="d5cd3-405">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="d5cd3-406">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-406">BatchAI</span></span>

* <span data-ttu-id="d5cd3-407">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="d5cd3-407">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="d5cd3-408">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-408">Container</span></span>

* <span data-ttu-id="d5cd3-409">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-409">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="d5cd3-410">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-410">IoT</span></span>

* <span data-ttu-id="d5cd3-411">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="d5cd3-411">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="d5cd3-412">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-412">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="d5cd3-413">Iot Central</span><span class="sxs-lookup"><span data-stu-id="d5cd3-413">Iot Central</span></span>

* <span data-ttu-id="d5cd3-414">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="d5cd3-414">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-415">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-415">KeyVault</span></span>


* <span data-ttu-id="d5cd3-416">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-416">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="d5cd3-417">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-417">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="d5cd3-418">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="d5cd3-418">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="d5cd3-419">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-419">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="d5cd3-420">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-420">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="d5cd3-421">Relais</span><span class="sxs-lookup"><span data-stu-id="d5cd3-421">Relay</span></span>

* <span data-ttu-id="d5cd3-422">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-422">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-423">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-423">Sql</span></span>

* <span data-ttu-id="d5cd3-424">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-424">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-425">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-425">Storage</span></span>

* <span data-ttu-id="d5cd3-426">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="d5cd3-426">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="d5cd3-427">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-427">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="d5cd3-428">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-428">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="d5cd3-429">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="d5cd3-429">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="d5cd3-430">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-430">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-431">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-431">VM</span></span>

* <span data-ttu-id="d5cd3-432">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-432">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="d5cd3-433">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-433">July 31, 2018</span></span>

<span data-ttu-id="d5cd3-434">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="d5cd3-434">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-435">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-435">ACR</span></span>

* <span data-ttu-id="d5cd3-436">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-436">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="d5cd3-437">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-437">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-438">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-438">ACS</span></span>

* <span data-ttu-id="d5cd3-439">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-439">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-440">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-440">Batch</span></span>

* <span data-ttu-id="d5cd3-441">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d5cd3-441">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-442">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-442">Container</span></span>

* <span data-ttu-id="d5cd3-443">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="d5cd3-443">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-444">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-444">Network</span></span>

* <span data-ttu-id="d5cd3-445">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5cd3-445">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="d5cd3-446">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-446">Resource</span></span>

* <span data-ttu-id="d5cd3-447">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-447">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="d5cd3-448">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-448">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-449">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-449">Role</span></span>

* <span data-ttu-id="d5cd3-450">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-450">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="d5cd3-451">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-451">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="d5cd3-452">Recherche</span><span class="sxs-lookup"><span data-stu-id="d5cd3-452">Search</span></span>

* <span data-ttu-id="d5cd3-453">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="d5cd3-453">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="d5cd3-454">Service Bus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-454">Service Bus</span></span>

* <span data-ttu-id="d5cd3-455">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="d5cd3-455">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="d5cd3-456">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-456">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="d5cd3-457">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-457">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="d5cd3-458">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-459">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-459">Storage</span></span>

* <span data-ttu-id="d5cd3-460">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-460">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="d5cd3-461">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-461">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-462">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-462">VM</span></span>

* <span data-ttu-id="d5cd3-463">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-463">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="d5cd3-464">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-464">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="d5cd3-465">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="d5cd3-465">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="d5cd3-466">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-466">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="d5cd3-467">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-467">July 18, 2018</span></span>

<span data-ttu-id="d5cd3-468">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="d5cd3-468">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-469">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-469">Core</span></span>

* <span data-ttu-id="d5cd3-470">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-470">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="d5cd3-471">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-471">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="d5cd3-472">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-472">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-473">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-473">ACR</span></span>

* <span data-ttu-id="d5cd3-474">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-474">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="d5cd3-475">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-475">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="d5cd3-476">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-476">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="d5cd3-477">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-477">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-478">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-478">ACS</span></span>

* <span data-ttu-id="d5cd3-479">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="d5cd3-479">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-480">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-480">AppService</span></span>

* <span data-ttu-id="d5cd3-481">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="d5cd3-481">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-482">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-482">Batch</span></span>

* <span data-ttu-id="d5cd3-483">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d5cd3-483">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="d5cd3-484">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="d5cd3-484">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d5cd3-485">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-485">Batch AI</span></span>

* <span data-ttu-id="d5cd3-486">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-486">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-487">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-487">Container</span></span>

* <span data-ttu-id="d5cd3-488">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="d5cd3-488">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="d5cd3-489">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="d5cd3-489">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-490">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-490">Network</span></span>

* <span data-ttu-id="d5cd3-491">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-491">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="d5cd3-492">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-492">Added `network nic wait`</span></span>
* <span data-ttu-id="d5cd3-493">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-493">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="d5cd3-494">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-494">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="d5cd3-495">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-495">Resource</span></span>

* <span data-ttu-id="d5cd3-496">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-496">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="d5cd3-497">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-497">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="d5cd3-498">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-498">Added `deployment wait` command</span></span>
* <span data-ttu-id="d5cd3-499">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d5cd3-499">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-500">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-500">SQL</span></span>

* <span data-ttu-id="d5cd3-501">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-501">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="d5cd3-502">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-502">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="d5cd3-503">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-503">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-504">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-504">Storage</span></span>

* <span data-ttu-id="d5cd3-505">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="d5cd3-505">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-506">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-506">VM</span></span>

* <span data-ttu-id="d5cd3-507">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-507">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="d5cd3-508">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-508">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="d5cd3-509">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-509">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d5cd3-510">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-510">July 3, 2018</span></span>

<span data-ttu-id="d5cd3-511">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="d5cd3-511">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="d5cd3-512">AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-512">AKS</span></span>

* <span data-ttu-id="d5cd3-513">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-513">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d5cd3-514">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-514">July 3, 2018</span></span>

<span data-ttu-id="d5cd3-515">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="d5cd3-515">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-516">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-516">Core</span></span>

* <span data-ttu-id="d5cd3-517">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-517">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-518">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-518">ACR</span></span>

* <span data-ttu-id="d5cd3-519">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="d5cd3-519">Added polling build status</span></span>
* <span data-ttu-id="d5cd3-520">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="d5cd3-520">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="d5cd3-521">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-521">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-522">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-522">ACS</span></span>

* <span data-ttu-id="d5cd3-523">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-523">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="d5cd3-524">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-524">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="d5cd3-525">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-525">Updated options for `aks browse` command.</span></span> <span data-ttu-id="d5cd3-526">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-526">Added `--listen-port` support</span></span>
* <span data-ttu-id="d5cd3-527">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-527">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="d5cd3-528">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="d5cd3-528">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="d5cd3-529">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-529">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-530">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-530">AppService</span></span>

* <span data-ttu-id="d5cd3-531">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-531">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="d5cd3-532">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="d5cd3-532">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="d5cd3-533">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="d5cd3-533">Backup</span></span>

* <span data-ttu-id="d5cd3-534">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="d5cd3-534">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="d5cd3-535">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-535">BatchAI</span></span>

* <span data-ttu-id="d5cd3-536">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-536">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="d5cd3-537">Cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-537">Cloud</span></span>

* <span data-ttu-id="d5cd3-538">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-538">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-539">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-539">Container</span></span>

* <span data-ttu-id="d5cd3-540">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="d5cd3-540">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="d5cd3-541">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-541">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="d5cd3-542">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="d5cd3-542">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-543">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-543">Extension</span></span>

* <span data-ttu-id="d5cd3-544">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-544">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-545">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-545">Network</span></span>

* <span data-ttu-id="d5cd3-546">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-546">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-547">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d5cd3-547">Rdbms</span></span>

* <span data-ttu-id="d5cd3-548">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-548">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-549">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-549">Resource</span></span>

* <span data-ttu-id="d5cd3-550">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-550">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-551">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-551">VM</span></span>

* <span data-ttu-id="d5cd3-552">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="d5cd3-552">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="d5cd3-553">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-553">June 25, 2018</span></span>

<span data-ttu-id="d5cd3-554">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="d5cd3-554">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="d5cd3-555">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-555">CLI</span></span>

* <span data-ttu-id="d5cd3-556">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-556">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="d5cd3-557">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-557">June 19, 2018</span></span>

<span data-ttu-id="d5cd3-558">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="d5cd3-558">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-559">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-559">Core</span></span>

* <span data-ttu-id="d5cd3-560">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-560">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-561">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-561">ACR</span></span>

* <span data-ttu-id="d5cd3-562">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="d5cd3-562">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="d5cd3-563">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-563">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-564">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-564">ACS</span></span>

* <span data-ttu-id="d5cd3-565">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-565">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="d5cd3-566">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-566">Added `--update` support</span></span>
* <span data-ttu-id="d5cd3-567">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-567">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="d5cd3-568">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-568">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="d5cd3-569">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-569">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="d5cd3-570">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-570">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="d5cd3-571">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-571">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="d5cd3-572">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-572">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-573">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-573">AppService</span></span>

* <span data-ttu-id="d5cd3-574">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-574">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="d5cd3-575">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-575">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-576">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-576">Batch</span></span>

* <span data-ttu-id="d5cd3-577">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-577">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d5cd3-578">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-578">Batch AI</span></span>

* <span data-ttu-id="d5cd3-579">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-579">Added support for workspaces.</span></span> <span data-ttu-id="d5cd3-580">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-580">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="d5cd3-581">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-581">Added support for experiments.</span></span> <span data-ttu-id="d5cd3-582">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-582">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="d5cd3-583">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="d5cd3-583">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="d5cd3-584">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-584">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="d5cd3-585">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-585">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="d5cd3-586">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-586">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="d5cd3-587">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-587">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="d5cd3-588">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="d5cd3-588">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="d5cd3-589">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-589">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="d5cd3-590">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-590">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="d5cd3-591">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-591">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="d5cd3-592">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-592">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="d5cd3-593">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-593">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="d5cd3-594">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-594">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="d5cd3-595">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-595">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="d5cd3-596">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-596">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="d5cd3-597">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-597">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="d5cd3-598">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-598">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d5cd3-599">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-599">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d5cd3-600">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-600">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="d5cd3-601">Cartes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-601">Maps</span></span>

* <span data-ttu-id="d5cd3-602">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-602">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-603">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-603">Network</span></span>

* <span data-ttu-id="d5cd3-604">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-604">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="d5cd3-605">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-605">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="d5cd3-606">#6502</span><span class="sxs-lookup"><span data-stu-id="d5cd3-606">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="d5cd3-607">Réservations</span><span class="sxs-lookup"><span data-stu-id="d5cd3-607">Reservations</span></span>

* <span data-ttu-id="d5cd3-608">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-608">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="d5cd3-609">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-609">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="d5cd3-610">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-610">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="d5cd3-611">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-611">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="d5cd3-612">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-612">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="d5cd3-613">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-613">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-614">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-614">Role</span></span>

* <span data-ttu-id="d5cd3-615">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-615">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-616">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-616">SQL</span></span>

* <span data-ttu-id="d5cd3-617">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-617">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-618">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-618">Storage</span></span>

* <span data-ttu-id="d5cd3-619">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-619">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-620">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-620">VM</span></span>

* <span data-ttu-id="d5cd3-621">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-621">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="d5cd3-622">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-622">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="d5cd3-623">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-623">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d5cd3-624">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-624">June 13, 2018</span></span>

<span data-ttu-id="d5cd3-625">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="d5cd3-625">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-626">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-626">Core</span></span>

* <span data-ttu-id="d5cd3-627">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-627">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d5cd3-628">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-628">June 13, 2018</span></span>

<span data-ttu-id="d5cd3-629">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d5cd3-629">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d5cd3-630">AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-630">AKS</span></span>

* <span data-ttu-id="d5cd3-631">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-631">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d5cd3-632">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="d5cd3-632">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="d5cd3-633">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-633">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d5cd3-634">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-634">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d5cd3-635">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-635">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-636">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-636">AppService</span></span>

* <span data-ttu-id="d5cd3-637">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="d5cd3-637">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d5cd3-638">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-638">June 5, 2018</span></span>

<span data-ttu-id="d5cd3-639">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d5cd3-639">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-640">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-640">Interactive</span></span>

* <span data-ttu-id="d5cd3-641">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-641">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d5cd3-642">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-642">June 5, 2018</span></span>

<span data-ttu-id="d5cd3-643">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d5cd3-643">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-644">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-644">Core</span></span>

* <span data-ttu-id="d5cd3-645">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="d5cd3-645">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d5cd3-646">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-646">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-647">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-647">ACR</span></span>

* <span data-ttu-id="d5cd3-648">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-648">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d5cd3-649">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-649">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d5cd3-650">AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-650">AKS</span></span>

* <span data-ttu-id="d5cd3-651">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-651">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-652">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-652">Batch</span></span>

* <span data-ttu-id="d5cd3-653">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-653">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-654">IOT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-654">IOT</span></span>

* <span data-ttu-id="d5cd3-655">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="d5cd3-655">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-656">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-656">Network</span></span>

* <span data-ttu-id="d5cd3-657">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="d5cd3-657">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d5cd3-658">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="d5cd3-658">Policy Insights</span></span>

* <span data-ttu-id="d5cd3-659">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-659">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d5cd3-660">ARM</span><span class="sxs-lookup"><span data-stu-id="d5cd3-660">ARM</span></span>

* <span data-ttu-id="d5cd3-661">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-661">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-662">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-662">SQL</span></span>

* <span data-ttu-id="d5cd3-663">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-663">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d5cd3-664">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-664">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d5cd3-665">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-665">Storage</span></span>

* <span data-ttu-id="d5cd3-666">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="d5cd3-666">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-667">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-667">VM</span></span>

* <span data-ttu-id="d5cd3-668">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-668">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d5cd3-669">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-669">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d5cd3-670">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-670">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d5cd3-671">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-671">May 22, 2018</span></span>

<span data-ttu-id="d5cd3-672">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d5cd3-672">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-673">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-673">Core</span></span>

* <span data-ttu-id="d5cd3-674">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="d5cd3-674">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-675">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-675">ACS</span></span>

* <span data-ttu-id="d5cd3-676">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-676">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d5cd3-677">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-677">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-678">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-678">AppService</span></span>

* <span data-ttu-id="d5cd3-679">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-679">Improved generic update commands</span></span>
* <span data-ttu-id="d5cd3-680">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-680">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-681">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-681">Container</span></span>

* <span data-ttu-id="d5cd3-682">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="d5cd3-682">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d5cd3-683">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-683">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-684">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-684">Extension</span></span>

* <span data-ttu-id="d5cd3-685">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-685">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-686">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-686">Interactive</span></span>

* <span data-ttu-id="d5cd3-687">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-687">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d5cd3-688">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="d5cd3-688">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-689">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-689">KeyVault</span></span>

* <span data-ttu-id="d5cd3-690">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="d5cd3-690">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-691">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-691">Network</span></span>

* <span data-ttu-id="d5cd3-692">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-692">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d5cd3-693">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-693">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-694">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-694">SQL</span></span>

* <span data-ttu-id="d5cd3-695">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-695">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d5cd3-696">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-696">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d5cd3-697">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-697">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="d5cd3-698">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="d5cd3-698">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d5cd3-699">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-699">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d5cd3-700">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-700">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d5cd3-701">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-701">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d5cd3-702">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-702">`edition`.</span></span> <span data-ttu-id="d5cd3-703">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-703">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d5cd3-704">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-704">`elasticPoolName`.</span></span> <span data-ttu-id="d5cd3-705">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-705">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d5cd3-706">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-706">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d5cd3-707">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-707">`edition`.</span></span> <span data-ttu-id="d5cd3-708">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-708">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d5cd3-709">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-709">`dtu`.</span></span> <span data-ttu-id="d5cd3-710">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-710">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d5cd3-711">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-711">`databaseDtuMin`.</span></span> <span data-ttu-id="d5cd3-712">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-712">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d5cd3-713">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-713">`databaseDtuMax`.</span></span> <span data-ttu-id="d5cd3-714">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-714">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d5cd3-715">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-715">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d5cd3-716">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-716">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-717">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-717">Storage</span></span>

* <span data-ttu-id="d5cd3-718">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-718">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d5cd3-719">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-719">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-720">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-720">VM</span></span>

* <span data-ttu-id="d5cd3-721">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-721">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d5cd3-722">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-722">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d5cd3-723">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-723">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d5cd3-724">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-724">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d5cd3-725">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-725">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d5cd3-726">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-726">May 7, 2018</span></span>

<span data-ttu-id="d5cd3-727">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d5cd3-727">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-728">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-728">Core</span></span>

* <span data-ttu-id="d5cd3-729">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="d5cd3-729">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d5cd3-730">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="d5cd3-730">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d5cd3-731">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-731">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d5cd3-732">#5591</span><span class="sxs-lookup"><span data-stu-id="d5cd3-732">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d5cd3-733">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-733">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d5cd3-734">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="d5cd3-734">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d5cd3-735">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-735">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d5cd3-736">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-736">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d5cd3-737">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-737">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-738">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-738">ACR</span></span>

* <span data-ttu-id="d5cd3-739">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-739">Added ACR Build commands</span></span>
* <span data-ttu-id="d5cd3-740">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="d5cd3-740">Improved resource not found error messages</span></span>
* <span data-ttu-id="d5cd3-741">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-741">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d5cd3-742">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-742">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d5cd3-743">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="d5cd3-743">Improved repository commands error messages</span></span>
* <span data-ttu-id="d5cd3-744">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-744">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-745">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-745">ACS</span></span>

* <span data-ttu-id="d5cd3-746">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="d5cd3-746">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d5cd3-747">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="d5cd3-747">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d5cd3-748">AMS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-748">AMS</span></span>

* <span data-ttu-id="d5cd3-749">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-749">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-750">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-750">Appservice</span></span>

* <span data-ttu-id="d5cd3-751">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="d5cd3-751">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d5cd3-752">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-752">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d5cd3-753">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="d5cd3-753">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d5cd3-754">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-754">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d5cd3-755">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-755">Batch AI</span></span>

* <span data-ttu-id="d5cd3-756">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="d5cd3-756">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d5cd3-757">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-757">Cognitive Services</span></span>

* <span data-ttu-id="d5cd3-758">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-758">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d5cd3-759">Consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-759">Consumption</span></span>

* <span data-ttu-id="d5cd3-760">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="d5cd3-760">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-761">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-761">Container</span></span>

* <span data-ttu-id="d5cd3-762">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-762">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d5cd3-763">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-763">Cosmos DB</span></span>

* <span data-ttu-id="d5cd3-764">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-764">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d5cd3-765">DMS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-765">DMS</span></span>

* <span data-ttu-id="d5cd3-766">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="d5cd3-766">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-767">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-767">Extension</span></span>

* <span data-ttu-id="d5cd3-768">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-768">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-769">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-769">Interactive</span></span>

* <span data-ttu-id="d5cd3-770">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-770">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d5cd3-771">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="d5cd3-771">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d5cd3-772">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-772">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d5cd3-773">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-773">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d5cd3-774">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-774">Lab</span></span>

* <span data-ttu-id="d5cd3-775">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="d5cd3-775">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-776">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-776">Network</span></span>

* <span data-ttu-id="d5cd3-777">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-777">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d5cd3-778">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-778">Profile</span></span>

* <span data-ttu-id="d5cd3-779">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-779">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d5cd3-780">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-780">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d5cd3-781">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-781">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d5cd3-782">Redis</span><span class="sxs-lookup"><span data-stu-id="d5cd3-782">Redis</span></span>

* <span data-ttu-id="d5cd3-783">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-783">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d5cd3-784">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-784">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d5cd3-785">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-785">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d5cd3-786">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-786">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d5cd3-787">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-787">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-788">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-788">Role</span></span>

* <span data-ttu-id="d5cd3-789">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-789">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-790">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-790">Storage</span></span>

* <span data-ttu-id="d5cd3-791">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-791">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d5cd3-792">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="d5cd3-792">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d5cd3-793">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-793">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d5cd3-794">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-794">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d5cd3-795">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-795">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-796">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-796">VM</span></span>

* <span data-ttu-id="d5cd3-797">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-797">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d5cd3-798">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-798">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d5cd3-799">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-799">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d5cd3-800">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-800">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d5cd3-801">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-801">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d5cd3-802">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="d5cd3-802">Added write accelerator support</span></span>
* <span data-ttu-id="d5cd3-803">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-803">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d5cd3-804">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-804">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d5cd3-805">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="d5cd3-805">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d5cd3-806">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-806">April 10, 2018</span></span>

<span data-ttu-id="d5cd3-807">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d5cd3-807">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-808">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-808">ACR</span></span>

* <span data-ttu-id="d5cd3-809">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="d5cd3-809">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-810">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-810">ACS</span></span>

* <span data-ttu-id="d5cd3-811">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="d5cd3-811">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-812">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-812">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d5cd3-814">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="d5cd3-814">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d5cd3-815">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-815">BatchAI</span></span>

* <span data-ttu-id="d5cd3-816">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="d5cd3-816">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="d5cd3-817">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-817">Job level mounting</span></span>
  - <span data-ttu-id="d5cd3-818">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="d5cd3-818">Environment variables with secret values</span></span>
  - <span data-ttu-id="d5cd3-819">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="d5cd3-819">Performance counters settings</span></span>
  - <span data-ttu-id="d5cd3-820">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-820">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="d5cd3-821">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="d5cd3-821">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="d5cd3-822">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="d5cd3-822">Usage and limits reporting</span></span>
  - <span data-ttu-id="d5cd3-823">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-823">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="d5cd3-824">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-824">Support for custom images</span></span>
  - <span data-ttu-id="d5cd3-825">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-825">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d5cd3-826">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-826">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d5cd3-827">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-827">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d5cd3-828">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-828">National clouds are supported</span></span>
* <span data-ttu-id="d5cd3-829">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="d5cd3-829">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d5cd3-830">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-830">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d5cd3-831">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-831">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d5cd3-832">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-832">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d5cd3-833">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-833">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d5cd3-834">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-834">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d5cd3-835">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-835">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d5cd3-836">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-836">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d5cd3-837">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="d5cd3-837">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d5cd3-838">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-838">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d5cd3-839">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-839">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d5cd3-840">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-840">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d5cd3-841">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-841">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d5cd3-842">Facturation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-842">Billing</span></span>

* <span data-ttu-id="d5cd3-843">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="d5cd3-843">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d5cd3-844">Consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-844">Consumption</span></span>

* <span data-ttu-id="d5cd3-845">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-845">Added `marketplace` commands</span></span>
* <span data-ttu-id="d5cd3-846">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-846">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d5cd3-847">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-847">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d5cd3-848">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-848">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d5cd3-849">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-849">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d5cd3-850">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-850">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-851">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-851">Container</span></span>

* <span data-ttu-id="d5cd3-852">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-852">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d5cd3-853">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="d5cd3-853">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-854">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-854">Extension</span></span>

* <span data-ttu-id="d5cd3-855">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-855">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-856">Interactive</span></span>

* <span data-ttu-id="d5cd3-857">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="d5cd3-857">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d5cd3-858">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-858">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d5cd3-859">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-859">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-860">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-860">Network</span></span>

* <span data-ttu-id="d5cd3-861">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="d5cd3-861">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d5cd3-862">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-862">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d5cd3-863">#4910</span><span class="sxs-lookup"><span data-stu-id="d5cd3-863">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d5cd3-864">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-864">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="d5cd3-865">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-865">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d5cd3-866">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-866">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d5cd3-867">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-867">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d5cd3-868">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-868">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-869">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-869">Profile</span></span>

* <span data-ttu-id="d5cd3-870">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-870">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d5cd3-871">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-871">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-872">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-872">RDBMS</span></span>

* <span data-ttu-id="d5cd3-873">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-873">Added `georestore` command</span></span>
* <span data-ttu-id="d5cd3-874">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-874">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-875">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-875">Resource</span></span>

* <span data-ttu-id="d5cd3-876">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-876">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d5cd3-877">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-877">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-878">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-878">SQL</span></span>

* <span data-ttu-id="d5cd3-879">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-879">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-880">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-880">Storage</span></span>

* <span data-ttu-id="d5cd3-881">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-881">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-882">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-882">VM</span></span>

* <span data-ttu-id="d5cd3-883">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-883">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d5cd3-884">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-884">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d5cd3-886">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-886">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d5cd3-887">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-887">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d5cd3-888">#5718</span><span class="sxs-lookup"><span data-stu-id="d5cd3-888">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d5cd3-889">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="d5cd3-889">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d5cd3-890">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-890">March 27, 2018</span></span>

<span data-ttu-id="d5cd3-891">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d5cd3-891">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-892">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-892">Core</span></span>

* <span data-ttu-id="d5cd3-893">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-893">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-894">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-894">ACS</span></span>

* <span data-ttu-id="d5cd3-895">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d5cd3-895">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-896">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-896">Appservice</span></span>

* <span data-ttu-id="d5cd3-897">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-897">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d5cd3-898">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-898">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d5cd3-899">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="d5cd3-899">Backup</span></span>

* <span data-ttu-id="d5cd3-900">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-900">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d5cd3-901">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-901">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d5cd3-902">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-902">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d5cd3-903">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-903">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-904">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-904">Container</span></span>

* <span data-ttu-id="d5cd3-905">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-905">Added `container exec` command.</span></span> <span data-ttu-id="d5cd3-906">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-906">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d5cd3-907">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-907">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-908">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-908">Extension</span></span>

* <span data-ttu-id="d5cd3-909">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="d5cd3-909">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d5cd3-910">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-910">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d5cd3-911">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-911">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-912">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-912">Interactive</span></span>

* <span data-ttu-id="d5cd3-913">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-913">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d5cd3-914">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-914">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d5cd3-915">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-915">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d5cd3-916">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="d5cd3-916">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d5cd3-917">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-917">Lab</span></span>

* <span data-ttu-id="d5cd3-918">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-918">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-919">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-919">Monitor</span></span>

* <span data-ttu-id="d5cd3-920">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-920">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d5cd3-921">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="d5cd3-921">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d5cd3-922">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-922">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-923">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-923">Network</span></span>

* <span data-ttu-id="d5cd3-924">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-924">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-925">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-925">Profile</span></span>

* <span data-ttu-id="d5cd3-926">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-926">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-927">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-927">RDBMS</span></span>

* <span data-ttu-id="d5cd3-928">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="d5cd3-928">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-929">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-929">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d5cd3-931">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-931">Role</span></span>

* <span data-ttu-id="d5cd3-932">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-932">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d5cd3-933">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="d5cd3-933">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d5cd3-934">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-934">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d5cd3-935">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-935">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d5cd3-936">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-936">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-937">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-937">Storage</span></span>

* <span data-ttu-id="d5cd3-938">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="d5cd3-938">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d5cd3-939">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="d5cd3-939">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-940">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-940">VM</span></span>

* <span data-ttu-id="d5cd3-941">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="d5cd3-941">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d5cd3-942">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-942">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d5cd3-943">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-943">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d5cd3-944">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-944">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d5cd3-945">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-945">March 13, 2018</span></span>

<span data-ttu-id="d5cd3-946">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d5cd3-946">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-947">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-947">ACR</span></span>

* <span data-ttu-id="d5cd3-948">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-948">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d5cd3-949">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-949">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d5cd3-950">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="d5cd3-950">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-951">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-951">ACS</span></span>

* <span data-ttu-id="d5cd3-952">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-952">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d5cd3-953">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-953">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d5cd3-954">Advisor</span><span class="sxs-lookup"><span data-stu-id="d5cd3-954">Advisor</span></span>

* <span data-ttu-id="d5cd3-955">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-955">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d5cd3-956">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-956">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d5cd3-957">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-957">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="d5cd3-958">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-958">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d5cd3-959">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-959">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-960">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-960">Appservice</span></span>

* <span data-ttu-id="d5cd3-961">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-961">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d5cd3-962">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-962">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d5cd3-963">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-963">Eventhubs</span></span>

* <span data-ttu-id="d5cd3-964">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-964">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-965">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-965">Extension</span></span>

* <span data-ttu-id="d5cd3-966">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-966">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-967">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-967">Interactive</span></span>

* <span data-ttu-id="d5cd3-968">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-968">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d5cd3-969">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-969">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d5cd3-970">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="d5cd3-970">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d5cd3-971">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="d5cd3-971">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-972">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-972">Monitor</span></span>

* <span data-ttu-id="d5cd3-973">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-973">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d5cd3-974">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-974">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d5cd3-975">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-975">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d5cd3-976">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-976">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-977">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-977">Network</span></span>

* <span data-ttu-id="d5cd3-978">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-978">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d5cd3-979">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-979">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d5cd3-980">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-980">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d5cd3-981">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-981">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-982">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-982">Profile</span></span>

* <span data-ttu-id="d5cd3-983">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-983">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d5cd3-984">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-984">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-985">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-985">RDBMS</span></span>

* <span data-ttu-id="d5cd3-986">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="d5cd3-986">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d5cd3-987">Service Bus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-987">Service Bus</span></span>

* <span data-ttu-id="d5cd3-988">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-988">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-989">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-989">Storage</span></span>

* <span data-ttu-id="d5cd3-990">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="d5cd3-990">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d5cd3-991">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="d5cd3-991">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-992">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-992">VM</span></span>

* <span data-ttu-id="d5cd3-993">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="d5cd3-993">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d5cd3-994">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-994">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d5cd3-995">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-995">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d5cd3-996">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="d5cd3-996">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d5cd3-997">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-997">February 27, 2018</span></span>

<span data-ttu-id="d5cd3-998">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d5cd3-998">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-999">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-999">Core</span></span>

* <span data-ttu-id="d5cd3-1000">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1000">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d5cd3-1001">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1001">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d5cd3-1002">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1002">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1003">ACS</span></span>

* <span data-ttu-id="d5cd3-1004">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1004">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d5cd3-1005">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1005">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d5cd3-1006">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1006">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d5cd3-1007">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1007">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1008">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1008">Appservice</span></span>

* <span data-ttu-id="d5cd3-1009">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1009">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d5cd3-1010">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1010">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d5cd3-1011">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1011">Cognitive Services</span></span>

* <span data-ttu-id="d5cd3-1012">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1012">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d5cd3-1013">Consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1013">Consumption</span></span>

* <span data-ttu-id="d5cd3-1014">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1014">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d5cd3-1015">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1015">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1016">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1016">Container</span></span>

* <span data-ttu-id="d5cd3-1017">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1017">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1018">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1018">Network</span></span>

* <span data-ttu-id="d5cd3-1019">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1019">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1020">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1020">Resource</span></span>

* <span data-ttu-id="d5cd3-1021">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1021">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1022">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1022">Role</span></span>

* <span data-ttu-id="d5cd3-1023">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1023">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1024">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1024">SQL</span></span>

* <span data-ttu-id="d5cd3-1025">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1025">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1026">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1026">Storage</span></span>

* <span data-ttu-id="d5cd3-1027">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1027">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1028">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1028">VM</span></span>

* <span data-ttu-id="d5cd3-1029">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1029">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d5cd3-1030">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1030">February 13, 2018</span></span>

<span data-ttu-id="d5cd3-1031">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1031">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1032">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1032">Core</span></span>

* <span data-ttu-id="d5cd3-1033">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1033">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1034">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1034">ACS</span></span>

* <span data-ttu-id="d5cd3-1035">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1035">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d5cd3-1036">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1036">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d5cd3-1037">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1037">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d5cd3-1038">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1038">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d5cd3-1039">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1039">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d5cd3-1040">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1040">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d5cd3-1041">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1041">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d5cd3-1042">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1042">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1043">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1043">Appservice</span></span>

* <span data-ttu-id="d5cd3-1044">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1044">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d5cd3-1045">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1045">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d5cd3-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1046">CDN</span></span>

* <span data-ttu-id="d5cd3-1047">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1047">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1048">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1048">Container</span></span>

* <span data-ttu-id="d5cd3-1049">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1049">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d5cd3-1050">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1050">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d5cd3-1051">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1051">CosmosDB</span></span>

* <span data-ttu-id="d5cd3-1052">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1052">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-1053">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1053">Extension</span></span>

* <span data-ttu-id="d5cd3-1054">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1054">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d5cd3-1055">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1055">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d5cd3-1056">Commentaires</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1056">Feedback</span></span>

* <span data-ttu-id="d5cd3-1057">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1057">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-1058">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1058">Interactive</span></span>

* <span data-ttu-id="d5cd3-1059">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1059">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d5cd3-1060">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1060">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-1061">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1061">IoT</span></span>

* <span data-ttu-id="d5cd3-1062">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1062">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d5cd3-1063">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1063">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d5cd3-1064">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1064">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1065">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1065">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1066">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1066">Monitor</span></span>

* <span data-ttu-id="d5cd3-1067">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1067">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1068">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1068">Network</span></span>

* <span data-ttu-id="d5cd3-1069">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1069">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d5cd3-1070">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1070">Profile</span></span>

* <span data-ttu-id="d5cd3-1071">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1071">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1072">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1072">Resource</span></span>

* <span data-ttu-id="d5cd3-1073">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1073">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1074">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1074">Role</span></span>

* <span data-ttu-id="d5cd3-1075">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1075">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1076">SQL</span></span>

* <span data-ttu-id="d5cd3-1077">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1077">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d5cd3-1078">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1078">Added `sql db rename`</span></span>
* <span data-ttu-id="d5cd3-1079">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1079">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1080">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1080">Storage</span></span>

* <span data-ttu-id="d5cd3-1081">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1081">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1082">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1082">VM</span></span>

* <span data-ttu-id="d5cd3-1083">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1083">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d5cd3-1084">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1084">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d5cd3-1085">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1085">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d5cd3-1086">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1086">January 31, 2018</span></span>

<span data-ttu-id="d5cd3-1087">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1087">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1088">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1088">Core</span></span>

* <span data-ttu-id="d5cd3-1089">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1089">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d5cd3-1090">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1090">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d5cd3-1091">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1091">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d5cd3-1092">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1092">Use `--verbose` to see</span></span>
* <span data-ttu-id="d5cd3-1093">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1093">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1094">ACS</span></span>

* <span data-ttu-id="d5cd3-1095">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1095">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d5cd3-1096">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1096">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1097">Appservice</span></span>

* <span data-ttu-id="d5cd3-1098">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1098">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d5cd3-1099">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1099">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d5cd3-1100">CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1100">CDN</span></span>

* <span data-ttu-id="d5cd3-1101">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1101">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d5cd3-1102">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1102">CosmosDB</span></span>

* <span data-ttu-id="d5cd3-1103">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1103">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-1104">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1104">Interactive</span></span>

* <span data-ttu-id="d5cd3-1105">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1105">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1106">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1106">Network</span></span>

* <span data-ttu-id="d5cd3-1107">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1107">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d5cd3-1108">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1108">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d5cd3-1109">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1109">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d5cd3-1110">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1110">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d5cd3-1111">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1111">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d5cd3-1112">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1112">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d5cd3-1113">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1113">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d5cd3-1114">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1114">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d5cd3-1115">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1115">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="d5cd3-1116">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1116">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1117">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1117">Profile</span></span>

* <span data-ttu-id="d5cd3-1118">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1118">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1119">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1119">Resource</span></span>

* <span data-ttu-id="d5cd3-1120">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1120">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1121">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1121">Storage</span></span>

* <span data-ttu-id="d5cd3-1122">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1122">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d5cd3-1123">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1123">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d5cd3-1124">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1124">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="d5cd3-1125">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1125">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d5cd3-1126">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1126">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1127">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1127">VM</span></span>

* <span data-ttu-id="d5cd3-1128">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1128">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d5cd3-1129">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1129">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d5cd3-1130">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1130">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d5cd3-1131">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1131">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d5cd3-1132">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1132">January 17, 2018</span></span>

<span data-ttu-id="d5cd3-1133">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1133">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1134">ACR</span></span>

* <span data-ttu-id="d5cd3-1135">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1135">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d5cd3-1136">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1136">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1137">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1137">ACS</span></span>

* <span data-ttu-id="d5cd3-1138">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1138">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d5cd3-1139">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1139">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1140">Appservice</span></span>

* <span data-ttu-id="d5cd3-1141">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1141">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d5cd3-1142">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1142">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d5cd3-1143">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1143">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d5cd3-1144">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1144">Backup</span></span>

* <span data-ttu-id="d5cd3-1145">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1145">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d5cd3-1146">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1146">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d5cd3-1147">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1147">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d5cd3-1148">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1148">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d5cd3-1149">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1149">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-1150">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1150">Batch</span></span>

* <span data-ttu-id="d5cd3-1151">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1151">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d5cd3-1152">Cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1152">Cloud</span></span>

* <span data-ttu-id="d5cd3-1153">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1153">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d5cd3-1154">Consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1154">Consumption</span></span>

* <span data-ttu-id="d5cd3-1155">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1155">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d5cd3-1156">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1156">Event Grid</span></span>

* <span data-ttu-id="d5cd3-1157">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1157">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d5cd3-1158">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1158">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d5cd3-1159">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1159">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d5cd3-1160">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1160">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d5cd3-1161">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1161">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d5cd3-1162">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1162">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d5cd3-1163">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1163">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d5cd3-1164">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1164">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-1165">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1165">Interactive</span></span>

* <span data-ttu-id="d5cd3-1166">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1166">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d5cd3-1167">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1167">Fixed errors on startup</span></span>
* <span data-ttu-id="d5cd3-1168">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1168">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-1169">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1169">IoT</span></span>

* <span data-ttu-id="d5cd3-1170">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1170">Added support for device provisioning service</span></span>
* <span data-ttu-id="d5cd3-1171">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1171">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d5cd3-1172">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1172">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1173">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1173">Monitor</span></span>

* <span data-ttu-id="d5cd3-1174">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1174">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d5cd3-1175">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1175">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d5cd3-1176">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1176">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1177">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1177">Network</span></span>

* <span data-ttu-id="d5cd3-1178">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1178">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d5cd3-1179">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1179">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1180">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1180">Profile</span></span>

* <span data-ttu-id="d5cd3-1181">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1181">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1182">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1182">Role</span></span>

* <span data-ttu-id="d5cd3-1183">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1183">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d5cd3-1184">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1184">Service Fabric</span></span>

* <span data-ttu-id="d5cd3-1185">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1185">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d5cd3-1186">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1186">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1187">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1187">VM</span></span>

* <span data-ttu-id="d5cd3-1188">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1188">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d5cd3-1189">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1189">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d5cd3-1190">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1190">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d5cd3-1191">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1191">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d5cd3-1192">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1192">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d5cd3-1193">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1193">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d5cd3-1194">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1194">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d5cd3-1195">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1195">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d5cd3-1196">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1196">December 19, 2017</span></span>

<span data-ttu-id="d5cd3-1197">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1197">Version 2.0.23</span></span>

* <span data-ttu-id="d5cd3-1198">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1198">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1199">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1199">Container</span></span>

* <span data-ttu-id="d5cd3-1200">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1200">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1201">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1201">Network</span></span>

* <span data-ttu-id="d5cd3-1202">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1202">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1203">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1203">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1204">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1204">Storage</span></span>

* <span data-ttu-id="d5cd3-1205">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1205">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1206">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1206">VM</span></span>

* <span data-ttu-id="d5cd3-1207">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1207">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d5cd3-1208">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1208">December 5, 2017</span></span>

<span data-ttu-id="d5cd3-1209">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1209">Version 2.0.22</span></span>

* <span data-ttu-id="d5cd3-1210">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1210">Removed `az component` commands.</span></span> <span data-ttu-id="d5cd3-1211">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1211">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1212">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1212">Core</span></span>
* <span data-ttu-id="d5cd3-1213">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1213">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d5cd3-1214">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1214">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1215">ACS</span></span>

* <span data-ttu-id="d5cd3-1216">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1216">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d5cd3-1217">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1217">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d5cd3-1218">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1218">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d5cd3-1219">Advisor</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1219">Advisor</span></span>

* <span data-ttu-id="d5cd3-1220">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1220">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1221">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1221">Appservice</span></span>

* <span data-ttu-id="d5cd3-1222">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1222">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d5cd3-1223">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1223">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d5cd3-1224">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1224">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d5cd3-1225">Consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1225">Consumption</span></span>

* <span data-ttu-id="d5cd3-1226">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1226">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1227">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1227">Container</span></span>

* <span data-ttu-id="d5cd3-1228">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1228">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1229">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1229">Monitor</span></span>

* <span data-ttu-id="d5cd3-1230">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1230">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1231">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1231">Resource</span></span>

* <span data-ttu-id="d5cd3-1232">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1232">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1233">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1233">Role</span></span>

* <span data-ttu-id="d5cd3-1234">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1234">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d5cd3-1235">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1235">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d5cd3-1236">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1236">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1237">SQL</span></span>

* <span data-ttu-id="d5cd3-1238">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1238">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d5cd3-1239">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1239">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1240">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1240">VM</span></span>

* <span data-ttu-id="d5cd3-1241">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1241">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d5cd3-1242">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1242">November 14, 2017</span></span>

<span data-ttu-id="d5cd3-1243">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1243">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-1244">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1244">ACR</span></span>

* <span data-ttu-id="d5cd3-1245">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1245">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d5cd3-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1246">ACS</span></span>

* <span data-ttu-id="d5cd3-1247">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1247">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d5cd3-1248">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1248">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d5cd3-1249">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1249">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d5cd3-1250">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1250">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d5cd3-1251">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1251">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1252">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1252">Appservice</span></span>

* <span data-ttu-id="d5cd3-1253">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1253">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d5cd3-1254">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1254">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d5cd3-1255">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1255">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d5cd3-1256">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1256">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d5cd3-1257">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1257">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d5cd3-1258">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1258">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-1259">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1259">Batch</span></span>

* <span data-ttu-id="d5cd3-1260">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1260">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d5cd3-1261">Batchai</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1261">Batchai</span></span>

* <span data-ttu-id="d5cd3-1262">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1262">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d5cd3-1263">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1263">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d5cd3-1264">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1264">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d5cd3-1265">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1265">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d5cd3-1266">Cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1266">Cloud</span></span>

* <span data-ttu-id="d5cd3-1267">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1267">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1268">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1268">Container</span></span>

* <span data-ttu-id="d5cd3-1269">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1269">Added support to open multiple ports</span></span>
* <span data-ttu-id="d5cd3-1270">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1270">Added container group restart policy</span></span>
* <span data-ttu-id="d5cd3-1271">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1271">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d5cd3-1272">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1272">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d5cd3-1273">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1273">Data Lake Analytics</span></span>

* <span data-ttu-id="d5cd3-1274">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1274">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d5cd3-1275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1275">Data Lake Store</span></span>

* <span data-ttu-id="d5cd3-1276">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1276">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-1277">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1277">Extension</span></span>

* <span data-ttu-id="d5cd3-1278">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1278">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d5cd3-1279">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1279">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-1280">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1280">IoT</span></span>

* <span data-ttu-id="d5cd3-1281">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1281">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1282">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1282">Monitor</span></span>

* <span data-ttu-id="d5cd3-1283">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1283">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1284">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1284">Network</span></span>

* <span data-ttu-id="d5cd3-1285">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1285">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d5cd3-1286">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1286">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d5cd3-1287">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1287">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d5cd3-1288">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1288">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d5cd3-1289">Réservations</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1289">Reservations</span></span>

* <span data-ttu-id="d5cd3-1290">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1290">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1291">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1291">Resource</span></span>

* <span data-ttu-id="d5cd3-1292">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1292">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1293">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1293">SQL</span></span>

* <span data-ttu-id="d5cd3-1294">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1294">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1295">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1295">Storage</span></span>

* <span data-ttu-id="d5cd3-1296">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1296">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d5cd3-1297">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1297">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d5cd3-1298">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1298">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d5cd3-1299">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1299">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d5cd3-1300">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1300">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d5cd3-1301">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1301">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d5cd3-1302">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1302">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1303">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1303">VM</span></span>

* <span data-ttu-id="d5cd3-1304">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1304">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d5cd3-1305">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1305">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d5cd3-1306">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1306">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d5cd3-1307">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1307">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d5cd3-1308">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1308">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d5cd3-1309">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1309">October 24, 2017</span></span>

<span data-ttu-id="d5cd3-1310">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1310">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1311">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1311">Core</span></span>

* <span data-ttu-id="d5cd3-1312">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1312">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1313">ACR</span></span>

* <span data-ttu-id="d5cd3-1314">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1314">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d5cd3-1315">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1315">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d5cd3-1316">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1316">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1317">ACS</span></span>

* <span data-ttu-id="d5cd3-1318">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1318">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d5cd3-1319">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1319">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1320">Appservice</span></span>

* <span data-ttu-id="d5cd3-1321">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1321">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d5cd3-1322">Composant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1322">Component</span></span>

* <span data-ttu-id="d5cd3-1323">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1323">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1324">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1324">Monitor</span></span>

* <span data-ttu-id="d5cd3-1325">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1325">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1326">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1326">Resource</span></span>

* <span data-ttu-id="d5cd3-1327">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1327">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d5cd3-1328">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1328">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1329">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1329">VM</span></span>

* <span data-ttu-id="d5cd3-1330">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1330">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d5cd3-1331">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1331">October 9, 2017</span></span>

<span data-ttu-id="d5cd3-1332">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1332">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1333">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1333">Core</span></span>

* <span data-ttu-id="d5cd3-1334">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1334">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1335">Appservice</span></span>

* <span data-ttu-id="d5cd3-1336">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1336">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-1337">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1337">Batch</span></span>

* <span data-ttu-id="d5cd3-1338">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1338">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d5cd3-1339">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1339">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d5cd3-1340">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1340">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d5cd3-1341">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1341">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d5cd3-1342">Batchai</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1342">Batchai</span></span>

* <span data-ttu-id="d5cd3-1343">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1343">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-1344">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1344">Keyvault</span></span>

* <span data-ttu-id="d5cd3-1345">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1345">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d5cd3-1346">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1346">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d5cd3-1347">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1347">Network</span></span>

* <span data-ttu-id="d5cd3-1348">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1348">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d5cd3-1349">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1349">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1350">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1350">Resource</span></span>

* <span data-ttu-id="d5cd3-1351">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1351">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d5cd3-1352">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1352">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d5cd3-1353">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1353">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d5cd3-1354">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1354">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1355">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1355">Sql</span></span>

* <span data-ttu-id="d5cd3-1356">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1356">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d5cd3-1357">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1357">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d5cd3-1358">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1358">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1359">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1359">Storage</span></span>

* <span data-ttu-id="d5cd3-1360">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1360">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1361">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1361">Vm</span></span>

* <span data-ttu-id="d5cd3-1362">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1362">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d5cd3-1363">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1363">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d5cd3-1364">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1364">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d5cd3-1365">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1365">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d5cd3-1366">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1366">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d5cd3-1367">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1367">September 22, 2017</span></span>

<span data-ttu-id="d5cd3-1368">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1368">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1369">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1369">Resource</span></span>

* <span data-ttu-id="d5cd3-1370">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1370">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d5cd3-1371">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1371">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d5cd3-1372">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1372">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d5cd3-1373">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1373">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1374">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1374">Network</span></span>

* <span data-ttu-id="d5cd3-1375">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1375">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d5cd3-1376">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1376">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d5cd3-1377">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1377">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d5cd3-1378">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1378">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d5cd3-1379">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1379">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1380">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1380">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1381">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1381">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1382">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1382">Storage</span></span>

* <span data-ttu-id="d5cd3-1383">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1383">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d5cd3-1384">Événement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1384">Eventgrid</span></span>

* <span data-ttu-id="d5cd3-1385">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1385">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1386">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1386">SQL</span></span>

* <span data-ttu-id="d5cd3-1387">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1387">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d5cd3-1388">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1388">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d5cd3-1389">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1389">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-1390">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1390">Keyvault</span></span>

* <span data-ttu-id="d5cd3-1391">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1391">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1392">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1392">VM</span></span>

* <span data-ttu-id="d5cd3-1393">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1393">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d5cd3-1394">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1394">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d5cd3-1395">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1395">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d5cd3-1396">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1396">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d5cd3-1397">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1397">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d5cd3-1398">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1398">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1399">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1399">ACS</span></span>

* <span data-ttu-id="d5cd3-1400">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1400">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1401">Appservice</span></span>

* <span data-ttu-id="d5cd3-1402">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1402">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d5cd3-1403">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1403">Backup</span></span>

* <span data-ttu-id="d5cd3-1404">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1404">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d5cd3-1405">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1405">September 11, 2017</span></span>

<span data-ttu-id="d5cd3-1406">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1406">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d5cd3-1407">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1407">Core</span></span>

* <span data-ttu-id="d5cd3-1408">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1408">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d5cd3-1409">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1409">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1410">Acs</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1410">Acs</span></span>

* <span data-ttu-id="d5cd3-1411">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1411">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d5cd3-1412">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1412">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1413">Appservice</span></span>

* <span data-ttu-id="d5cd3-1414">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1414">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d5cd3-1415">CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1415">CDN</span></span>

* <span data-ttu-id="d5cd3-1416">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1416">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d5cd3-1417">Extension</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1417">Extension</span></span>

* <span data-ttu-id="d5cd3-1418">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1418">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-1419">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1419">Keyvault</span></span>

* <span data-ttu-id="d5cd3-1420">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1420">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1421">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1421">Network</span></span>

* <span data-ttu-id="d5cd3-1422">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1422">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d5cd3-1423">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1423">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d5cd3-1424">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1424">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d5cd3-1425">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1425">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d5cd3-1426">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1426">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1427">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1427">Resource</span></span>

* <span data-ttu-id="d5cd3-1428">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1428">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d5cd3-1429">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1429">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d5cd3-1430">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1430">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d5cd3-1431">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1431">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1432">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1432">SQL</span></span>

* <span data-ttu-id="d5cd3-1433">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1433">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1434">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1434">VM</span></span>

* <span data-ttu-id="d5cd3-1435">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1435">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d5cd3-1436">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1436">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d5cd3-1437">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1437">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d5cd3-1438">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1438">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d5cd3-1439">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1439">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d5cd3-1440">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1440">August 31, 2017</span></span>

<span data-ttu-id="d5cd3-1441">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1441">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-1442">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1442">Keyvault</span></span>

* <span data-ttu-id="d5cd3-1443">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1443">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d5cd3-1444">Sf</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1444">Sf</span></span>

* <span data-ttu-id="d5cd3-1445">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1445">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1446">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1446">Storage</span></span>

* <span data-ttu-id="d5cd3-1447">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1447">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d5cd3-1448">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1448">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d5cd3-1449">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1449">August 28, 2017</span></span>

<span data-ttu-id="d5cd3-1450">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1450">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d5cd3-1451">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1451">CLI</span></span>

* <span data-ttu-id="d5cd3-1452">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1452">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1453">ACS</span></span>

* <span data-ttu-id="d5cd3-1454">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1454">Corrected preview regions</span></span>
* <span data-ttu-id="d5cd3-1455">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1455">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d5cd3-1456">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1456">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1457">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1457">Appservice</span></span>

* <span data-ttu-id="d5cd3-1458">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1458">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d5cd3-1459">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1459">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d5cd3-1460">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1460">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d5cd3-1461">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1461">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d5cd3-1462">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1462">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-1463">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1463">IoT</span></span>

* <span data-ttu-id="d5cd3-1464">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1464">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1465">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1465">Network</span></span>

* <span data-ttu-id="d5cd3-1466">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1466">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d5cd3-1467">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1467">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1468">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1468">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d5cd3-1469">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d5cd3-1470">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1470">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1471">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1471">Profile</span></span>

* <span data-ttu-id="d5cd3-1472">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1472">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d5cd3-1473">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1473">Service Fabric</span></span>

* <span data-ttu-id="d5cd3-1474">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1474">Preview release</span></span>
* <span data-ttu-id="d5cd3-1475">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1475">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d5cd3-1476">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1476">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d5cd3-1477">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1477">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1478">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1478">Storage</span></span>

* <span data-ttu-id="d5cd3-1479">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1479">Enabled setting blob tier</span></span>
* <span data-ttu-id="d5cd3-1480">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1480">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d5cd3-1481">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1481">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d5cd3-1482">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1482">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d5cd3-1483">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1483">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d5cd3-1484">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1484">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1485">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1485">VM</span></span>

* <span data-ttu-id="d5cd3-1486">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1486">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d5cd3-1487">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1487">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d5cd3-1488">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1488">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d5cd3-1489">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1489">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d5cd3-1490">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1490">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d5cd3-1491">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1491">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d5cd3-1492">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1492">August 15, 2017</span></span>

<span data-ttu-id="d5cd3-1493">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1493">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1494">ACS</span></span>

* <span data-ttu-id="d5cd3-1495">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1495">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1496">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1496">Appservice</span></span>

* <span data-ttu-id="d5cd3-1497">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1497">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d5cd3-1498">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1498">Event Grid</span></span>

* <span data-ttu-id="d5cd3-1499">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1499">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d5cd3-1500">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1500">August 11, 2017</span></span>

<span data-ttu-id="d5cd3-1501">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1501">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1502">ACS</span></span>

* <span data-ttu-id="d5cd3-1503">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1503">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-1504">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1504">Batch</span></span>

* <span data-ttu-id="d5cd3-1505">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1505">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d5cd3-1506">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1506">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d5cd3-1507">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1507">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d5cd3-1508">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1508">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d5cd3-1509">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1509">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d5cd3-1510">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1510">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d5cd3-1511">Composant</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1511">Component</span></span>

* <span data-ttu-id="d5cd3-1512">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1512">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d5cd3-1513">Conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1513">Container</span></span>

* <span data-ttu-id="d5cd3-1514">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1514">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d5cd3-1515">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1515">Data Lake Store</span></span>

* <span data-ttu-id="d5cd3-1516">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1516">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d5cd3-1517">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1517">Event Grid</span></span>

* <span data-ttu-id="d5cd3-1518">Version initiale</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1518">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1519">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1519">Network</span></span>

* <span data-ttu-id="d5cd3-1520">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1520">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d5cd3-1521">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1521">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d5cd3-1522">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1522">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d5cd3-1523">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1523">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1524">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1524">Profile</span></span>

* <span data-ttu-id="d5cd3-1525">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1525">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1526">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1526">Storage</span></span>

* <span data-ttu-id="d5cd3-1527">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1527">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1528">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1528">VM</span></span>

* <span data-ttu-id="d5cd3-1529">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1529">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d5cd3-1530">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1530">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d5cd3-1531">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1531">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d5cd3-1532">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1532">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d5cd3-1533">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1533">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d5cd3-1534">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1534">July 28, 2017</span></span>

<span data-ttu-id="d5cd3-1535">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1535">Version 2.0.12</span></span>

* <span data-ttu-id="d5cd3-1536">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1536">Added container commands</span></span>
* <span data-ttu-id="d5cd3-1537">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1537">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d5cd3-1538">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1538">Core</span></span>

* <span data-ttu-id="d5cd3-1539">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1539">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d5cd3-1540">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1540">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d5cd3-1541">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1541">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d5cd3-1542">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1542">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d5cd3-1543">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1543">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d5cd3-1544">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1544">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d5cd3-1545">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1545">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d5cd3-1546">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1546">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d5cd3-1547">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1547">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d5cd3-1548">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1548">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d5cd3-1549">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1549">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d5cd3-1550">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1550">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d5cd3-1551">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1551">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d5cd3-1552">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1552">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d5cd3-1553">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1553">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d5cd3-1554">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1554">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d5cd3-1555">ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1555">ACR</span></span>

* <span data-ttu-id="d5cd3-1556">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1556">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d5cd3-1557">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1557">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d5cd3-1558">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1558">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d5cd3-1559">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1559">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d5cd3-1560">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1560">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d5cd3-1561">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1561">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1562">ACS</span></span>

* <span data-ttu-id="d5cd3-1563">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1563">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1564">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1564">Appservice</span></span>

* <span data-ttu-id="d5cd3-1565">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1565">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d5cd3-1566">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1566">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d5cd3-1567">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1567">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d5cd3-1568">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1568">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d5cd3-1569">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1569">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d5cd3-1570">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1570">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d5cd3-1571">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1571">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d5cd3-1572">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1572">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d5cd3-1573">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1573">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d5cd3-1574">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1574">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d5cd3-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1575">Batch</span></span>

* <span data-ttu-id="d5cd3-1576">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1576">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d5cd3-1577">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1577">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d5cd3-1578">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1578">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d5cd3-1579">CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1579">CDN</span></span>

* <span data-ttu-id="d5cd3-1580">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1580">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d5cd3-1581">Cloud</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1581">Cloud</span></span>

* <span data-ttu-id="d5cd3-1582">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1582">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d5cd3-1583">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1583">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d5cd3-1584">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1584">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d5cd3-1585">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1585">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d5cd3-1586">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1586">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d5cd3-1587">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1587">CosmosDB</span></span>

* <span data-ttu-id="d5cd3-1588">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1588">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d5cd3-1589">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1589">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d5cd3-1590">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1590">Data Lake Analytics</span></span>

* <span data-ttu-id="d5cd3-1591">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1591">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d5cd3-1592">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1592">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d5cd3-1593">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1593">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d5cd3-1594">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1594">Data Lake Store</span></span>

* <span data-ttu-id="d5cd3-1595">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1595">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d5cd3-1596">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1596">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d5cd3-1597">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1597">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d5cd3-1598">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1598">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d5cd3-1599">Interactive</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1599">Interactive</span></span>

* <span data-ttu-id="d5cd3-1600">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1600">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d5cd3-1601">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1601">Increased test coverage</span></span>
* <span data-ttu-id="d5cd3-1602">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1602">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d5cd3-1603">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1603">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d5cd3-1604">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1604">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d5cd3-1605">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1605">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d5cd3-1606">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1606">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d5cd3-1607">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1607">Added `--progress` flag</span></span>
* <span data-ttu-id="d5cd3-1608">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1608">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d5cd3-1609">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1609">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d5cd3-1610">IoT</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1610">IoT</span></span>

* <span data-ttu-id="d5cd3-1611">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1611">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d5cd3-1612">(#3934)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1612">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d5cd3-1613">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1613">Key vault</span></span>

* <span data-ttu-id="d5cd3-1614">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1614">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d5cd3-1615">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1615">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d5cd3-1616">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1616">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d5cd3-1617">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1617">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d5cd3-1618">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1618">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d5cd3-1619">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1619">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d5cd3-1620">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1620">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d5cd3-1621">(#3307)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1621">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d5cd3-1622">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1622">Lab</span></span>

* <span data-ttu-id="d5cd3-1623">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1623">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d5cd3-1624">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1624">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1625">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1625">Monitor</span></span>

* <span data-ttu-id="d5cd3-1626">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1626">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d5cd3-1627">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1627">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d5cd3-1628">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1628">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d5cd3-1629">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1629">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d5cd3-1630">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1630">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d5cd3-1631">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1631">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d5cd3-1632">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1632">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d5cd3-1633">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1633">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d5cd3-1634">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1634">`location` no longer required</span></span>
  * <span data-ttu-id="d5cd3-1635">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1635">Add name and ID support for target</span></span>
  * <span data-ttu-id="d5cd3-1636">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1636">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d5cd3-1637">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1637">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d5cd3-1638">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1638">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d5cd3-1639">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1639">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d5cd3-1640">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1640">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d5cd3-1641">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1641">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1642">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1642">Network</span></span>

* <span data-ttu-id="d5cd3-1643">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1643">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d5cd3-1644">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1644">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d5cd3-1645">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1645">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d5cd3-1646">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1646">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d5cd3-1647">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1647">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d5cd3-1648">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1648">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d5cd3-1649">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1649">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d5cd3-1650">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1650">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d5cd3-1651">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1651">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d5cd3-1652">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1652">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d5cd3-1653">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1653">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d5cd3-1654">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1654">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d5cd3-1655">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1655">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d5cd3-1656">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1656">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d5cd3-1657">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1657">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d5cd3-1658">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1658">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d5cd3-1659">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1659">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d5cd3-1660">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1660">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d5cd3-1661">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1661">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d5cd3-1662">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1662">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d5cd3-1663">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1663">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d5cd3-1664">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1664">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d5cd3-1665">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1665">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d5cd3-1666">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1666">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d5cd3-1667">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1667">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d5cd3-1668">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1668">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d5cd3-1669">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1669">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1670">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1670">Profile</span></span>

* <span data-ttu-id="d5cd3-1671">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1671">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d5cd3-1672">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1672">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d5cd3-1673">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1673">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d5cd3-1674">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1674">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d5cd3-1675">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1675">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d5cd3-1676">SGBDR</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1676">RDBMS</span></span>

* <span data-ttu-id="d5cd3-1677">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1677">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d5cd3-1678">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1678">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d5cd3-1679">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1679">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d5cd3-1680">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1680">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1681">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1681">Resource</span></span>

* <span data-ttu-id="d5cd3-1682">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1682">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d5cd3-1683">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1683">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d5cd3-1684">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1684">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d5cd3-1685">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1685">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d5cd3-1686">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1686">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d5cd3-1687">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1687">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d5cd3-1688">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1688">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d5cd3-1689">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1689">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1690">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1690">Role</span></span>

* <span data-ttu-id="d5cd3-1691">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1691">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d5cd3-1692">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1692">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d5cd3-1693">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1693">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d5cd3-1694">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1694">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d5cd3-1695">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1695">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d5cd3-1696">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1696">Service Fabric</span></span>
* <span data-ttu-id="d5cd3-1697">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1697">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d5cd3-1698">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1698">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d5cd3-1699">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1699">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1700">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1700">SQL</span></span>

* <span data-ttu-id="d5cd3-1701">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1701">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d5cd3-1702">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1702">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d5cd3-1703">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1703">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1704">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1704">Storage</span></span>

* <span data-ttu-id="d5cd3-1705">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1705">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d5cd3-1706">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1706">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d5cd3-1707">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1707">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d5cd3-1708">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1708">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d5cd3-1709">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1709">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d5cd3-1710">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1710">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1711">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1711">VM</span></span>

* <span data-ttu-id="d5cd3-1712">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1712">Support configuring nsg</span></span>
* <span data-ttu-id="d5cd3-1713">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1713">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d5cd3-1714">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1714">Support managed service identities</span></span>
* <span data-ttu-id="d5cd3-1715">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1715">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d5cd3-1716">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1716">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d5cd3-1717">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1717">May 10, 2017</span></span>

<span data-ttu-id="d5cd3-1718">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1718">Version 2.0.6</span></span>

* <span data-ttu-id="d5cd3-1719">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1719">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d5cd3-1720">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1720">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d5cd3-1721">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1721">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d5cd3-1722">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1722">Include Cognitive Services module</span></span>
* <span data-ttu-id="d5cd3-1723">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1723">Include Service Fabric module</span></span>
* <span data-ttu-id="d5cd3-1724">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1724">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d5cd3-1725">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1725">Add support for CDN commands</span></span>
* <span data-ttu-id="d5cd3-1726">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1726">Remove Container module</span></span>
* <span data-ttu-id="d5cd3-1727">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1727">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d5cd3-1728">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1728">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d5cd3-1729">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1729">Core</span></span>

* <span data-ttu-id="d5cd3-1730">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1730">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d5cd3-1731">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1731">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d5cd3-1732">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1732">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d5cd3-1733">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1733">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d5cd3-1734">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1734">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d5cd3-1735">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1735">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d5cd3-1736">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1736">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d5cd3-1737">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1737">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d5cd3-1738">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1738">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d5cd3-1739">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1739">core: Improved performance</span></span>
* <span data-ttu-id="d5cd3-1740">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1740">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d5cd3-1741">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1741">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1742">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1742">ACS</span></span>

* <span data-ttu-id="d5cd3-1743">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1743">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d5cd3-1744">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1744">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d5cd3-1745">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1745">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d5cd3-1746">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1746">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1747">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1747">AppService</span></span>

* <span data-ttu-id="d5cd3-1748">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1748">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d5cd3-1749">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1749">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d5cd3-1750">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1750">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d5cd3-1751">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1751">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d5cd3-1752">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1752">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d5cd3-1753">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1753">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d5cd3-1754">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1754">support slot swap with preview</span></span>
* <span data-ttu-id="d5cd3-1755">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1755">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d5cd3-1756">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1756">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d5cd3-1757">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1757">CosmosDB</span></span>

* <span data-ttu-id="d5cd3-1758">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1758">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d5cd3-1759">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1759">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d5cd3-1760">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1760">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d5cd3-1761">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1761">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d5cd3-1762">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1762">Data Lake Analytics</span></span>

* <span data-ttu-id="d5cd3-1763">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1763">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d5cd3-1764">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1764">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d5cd3-1765">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1765">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d5cd3-1766">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1766">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d5cd3-1767">Table</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1767">Table</span></span>
  * <span data-ttu-id="d5cd3-1768">Fonction table</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1768">Table valued function</span></span>
  * <span data-ttu-id="d5cd3-1769">Affichage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1769">View</span></span>
  * <span data-ttu-id="d5cd3-1770">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1770">Table Statistics.</span></span> <span data-ttu-id="d5cd3-1771">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1771">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d5cd3-1772">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1772">Data Lake Store</span></span>

* <span data-ttu-id="d5cd3-1773">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1773">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d5cd3-1774">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1774">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d5cd3-1775">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1775">missed help for access show.</span></span> <span data-ttu-id="d5cd3-1776">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1776">adding it.</span></span> <span data-ttu-id="d5cd3-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d5cd3-1778">Rechercher</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1778">Find</span></span>

* <span data-ttu-id="d5cd3-1779">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1779">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5cd3-1780">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1780">KeyVault</span></span>

* <span data-ttu-id="d5cd3-1781">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1781">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d5cd3-1782">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1782">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d5cd3-1783">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1783">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d5cd3-1784">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1784">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d5cd3-1785">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1785">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d5cd3-1786">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1786">Lab</span></span>

* <span data-ttu-id="d5cd3-1787">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1787">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d5cd3-1788">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1788">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d5cd3-1789">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1789">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d5cd3-1790">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1790">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d5cd3-1791">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1791">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d5cd3-1792">Surveiller</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1792">Monitor</span></span>

* <span data-ttu-id="d5cd3-1793">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1793">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d5cd3-1794">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1794">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d5cd3-1795">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1795">Network</span></span>

* <span data-ttu-id="d5cd3-1796">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1796">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d5cd3-1797">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1797">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d5cd3-1798">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1798">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d5cd3-1799">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1799">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d5cd3-1800">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1800">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d5cd3-1801">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1801">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d5cd3-1802">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1802">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d5cd3-1803">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1803">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d5cd3-1804">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1804">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d5cd3-1805">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1805">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d5cd3-1806">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1806">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d5cd3-1807">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1807">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d5cd3-1808">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1808">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d5cd3-1809">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1809">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d5cd3-1810">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1810">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d5cd3-1811">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1811">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d5cd3-1812">Profil</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1812">Profile</span></span>

* <span data-ttu-id="d5cd3-1813">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1813">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d5cd3-1814">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1814">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d5cd3-1815">Redis</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1815">Redis</span></span>

* <span data-ttu-id="d5cd3-1816">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1816">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d5cd3-1817">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1817">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d5cd3-1818">Ressource</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1818">Resource</span></span>

* <span data-ttu-id="d5cd3-1819">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1819">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d5cd3-1820">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1820">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d5cd3-1821">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1821">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d5cd3-1822">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1822">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d5cd3-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d5cd3-1824">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1824">Add docs for az lock update.</span></span> <span data-ttu-id="d5cd3-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d5cd3-1826">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1826">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d5cd3-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d5cd3-1828">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1828">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d5cd3-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d5cd3-1830">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1830">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d5cd3-1831">Rôle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1831">Role</span></span>

* <span data-ttu-id="d5cd3-1832">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1832">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d5cd3-1833">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1833">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d5cd3-1834">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1834">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d5cd3-1835">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1835">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d5cd3-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1836">SQL</span></span>

* <span data-ttu-id="d5cd3-1837">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1837">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d5cd3-1838">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1838">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d5cd3-1839">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1839">Storage</span></span>

* <span data-ttu-id="d5cd3-1840">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1840">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d5cd3-1841">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1841">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d5cd3-1842">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1842">Add support for large block blob upload</span></span>
* <span data-ttu-id="d5cd3-1843">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1843">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1844">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1844">VM</span></span>

* <span data-ttu-id="d5cd3-1845">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1845">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d5cd3-1846">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1846">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d5cd3-1847">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1847">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d5cd3-1848">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1848">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d5cd3-1849">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1849">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d5cd3-1850">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1850">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d5cd3-1851">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1851">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d5cd3-1852">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1852">April 3, 2017</span></span>

<span data-ttu-id="d5cd3-1853">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1853">Version 2.0.2</span></span>

<span data-ttu-id="d5cd3-1854">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1854">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d5cd3-1855">Principal</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1855">Core</span></span>

* <span data-ttu-id="d5cd3-1856">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1856">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d5cd3-1857">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1857">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d5cd3-1858">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1858">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d5cd3-1859">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1859">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d5cd3-1860">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1860">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d5cd3-1861">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1861">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d5cd3-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d5cd3-1863">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1863">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d5cd3-1864">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1864">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d5cd3-1865">ACS</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1865">ACS</span></span>

* <span data-ttu-id="d5cd3-1866">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1866">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d5cd3-1867">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1867">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d5cd3-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d5cd3-1869">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1869">Add support for windows clusters.</span></span> <span data-ttu-id="d5cd3-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d5cd3-1871">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1871">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d5cd3-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d5cd3-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1873">AppService</span></span>

* <span data-ttu-id="d5cd3-1874">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1874">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d5cd3-1875">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1875">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d5cd3-1876">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1876">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d5cd3-1877">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1877">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d5cd3-1878">DataLake</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1878">DataLake</span></span>

* <span data-ttu-id="d5cd3-1879">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1879">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d5cd3-1880">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1880">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d5cd3-1881">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1881">DocuemntDB</span></span>

* <span data-ttu-id="d5cd3-1882">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1882">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d5cd3-1883">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1883">VM</span></span>

* <span data-ttu-id="d5cd3-1884">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1884">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d5cd3-1885">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1885">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d5cd3-1886">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1886">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d5cd3-1887">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1887">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d5cd3-1888">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1888">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d5cd3-1889">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1889">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="d5cd3-1890">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1890">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d5cd3-1891">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1891">February 27, 2017</span></span>

<span data-ttu-id="d5cd3-1892">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1892">Version 2.0.0</span></span>

<span data-ttu-id="d5cd3-1893">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1893">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d5cd3-1894">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1894">Container Service (acs)</span></span>
- <span data-ttu-id="d5cd3-1895">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1895">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d5cd3-1896">Réseau</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1896">Networking</span></span>
- <span data-ttu-id="d5cd3-1897">Stockage</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1897">Storage</span></span>

<span data-ttu-id="d5cd3-1898">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1898">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d5cd3-1899">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1899">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d5cd3-1900">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1900">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d5cd3-1901">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1901">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d5cd3-1902">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1902">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d5cd3-1903">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1903">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d5cd3-1904">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1904">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d5cd3-1905">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1905">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d5cd3-1906">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="d5cd3-1906">Provide feedback from the command line with the `az feedback` command</span></span>

