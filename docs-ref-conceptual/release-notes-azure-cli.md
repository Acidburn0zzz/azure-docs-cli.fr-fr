---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/09/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: df665565130322504c4794462098980b1064a6c7
ms.sourcegitcommit: c6dff58438d256647d4aa29a53eef4bf93a0cd24
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/11/2019
ms.locfileid: "59479995"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="a0e85-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a0e85-103">Azure CLI release notes</span></span>
## <a name="april-9-2019"></a><span data-ttu-id="a0e85-104">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-104">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-105">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-105">Core</span></span>
* <span data-ttu-id="a0e85-106">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="a0e85-106">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-107">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-107">ACR</span></span>
* <span data-ttu-id="a0e85-108">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="a0e85-108">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="a0e85-109">AMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-109">AMS</span></span>
* [<span data-ttu-id="a0e85-110">DÉPRÉCIÉ</span><span class="sxs-lookup"><span data-stu-id="a0e85-110">DEPRECATED</span></span>]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [<span data-ttu-id="a0e85-111">CHANGEMENT CASSANT</span><span class="sxs-lookup"><span data-stu-id="a0e85-111">BREAKING CHANGE</span></span>]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="a0e85-112">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-112">Added new encryption parameters support in</span></span> `ams streaming-policy create`
* <span data-ttu-id="a0e85-113">Ajout du nouveau paramètre `--filters` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-113">Added new paramter `--filters` to</span></span> `ams streaming-locator create`

### <a name="appservice"></a><span data-ttu-id="a0e85-114">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-114">AppService</span></span>
* <span data-ttu-id="a0e85-115">Ajout de la prise en charge de `--logs` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-115">Added `--logs` support to</span></span> `webapp up`
* <span data-ttu-id="a0e85-116">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-116">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="a0e85-117">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-117">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="a0e85-118">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a0e85-118">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="a0e85-119">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-119">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="a0e85-120">Ajout de la possibilité de basculer un plan sous une application de fonction avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-120">Added ability to switch a plan underneath a function app using</span></span> `functionapp update --plan`
* <span data-ttu-id="a0e85-121">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="a0e85-121">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="a0e85-122">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-122">CDN</span></span>
* <span data-ttu-id="a0e85-123">Ajout de la prise en charge de `Microsoft_Standard` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-123">Added support for `Microsoft_Standard` and</span></span> `Standard_ChinaCdn`

### <a name="feedback"></a><span data-ttu-id="a0e85-124">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a0e85-124">Feedback</span></span>
* <span data-ttu-id="a0e85-125">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="a0e85-125">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="a0e85-126">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="a0e85-126">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="a0e85-127">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="a0e85-127">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-128">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-128">Monitor</span></span>
* <span data-ttu-id="a0e85-129">Correction du problème où « count » n’était pas une valeur autorisée avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-129">Fixed issue where "count" was not a permitted value with</span></span> `metrics alert [create|update]` 

### <a name="network"></a><span data-ttu-id="a0e85-130">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-130">Network</span></span>
* <span data-ttu-id="a0e85-131">Correction du problème empêchant l’affichage du format de table avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-131">Fixed table format not displaying with</span></span> `vnet-gateway list-bgp-peer-status`
* <span data-ttu-id="a0e85-132">Ajout des commandes `list-request-headers` et `list-response-headers` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-132">Added `list-request-headers` and `list-response-headers` commands to</span></span> `application-gateway rewrite-rule`
* <span data-ttu-id="a0e85-133">Ajout de la commande `list-server-variables` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-133">Added `list-server-variables` command to</span></span> `application-gateway rewrite-rule condition`
* <span data-ttu-id="a0e85-134">Correction d’un problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu</span><span class="sxs-lookup"><span data-stu-id="a0e85-134">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception</span></span> `express-route port update`

### <a name="privatedns"></a><span data-ttu-id="a0e85-135">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="a0e85-135">PrivateDNS</span></span>
* <span data-ttu-id="a0e85-136">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="a0e85-136">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-137">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-137">Resource</span></span>
* <span data-ttu-id="a0e85-138">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-138">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-139">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-139">Role</span></span>
* <span data-ttu-id="a0e85-140">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-140">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="a0e85-141">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-141">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-142">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-142">SQL</span></span>
* <span data-ttu-id="a0e85-143">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="a0e85-143">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-144">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-144">Storage</span></span>
* <span data-ttu-id="a0e85-145">[CHANGEMENT CASSANT] Suppression du résultat de</span><span class="sxs-lookup"><span data-stu-id="a0e85-145">[BREAKING CHANGE] Removed result of</span></span> `storage blob delete`
* <span data-ttu-id="a0e85-146">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="a0e85-146">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="a0e85-147">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="a0e85-147">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="a0e85-148">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="a0e85-148">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="a0e85-149">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-149">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="a0e85-150">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-150">Core</span></span>
* <span data-ttu-id="a0e85-151">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="a0e85-151">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="a0e85-152">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="a0e85-152">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="a0e85-153">Cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-153">Cloud</span></span>
* <span data-ttu-id="a0e85-154">Correction d’une erreur « abonnement introuvable » dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-154">Fixed a 'subscription not found' error in</span></span> `cloud set`

### <a name="acr"></a><span data-ttu-id="a0e85-155">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-155">ACR</span></span>
* <span data-ttu-id="a0e85-156">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="a0e85-156">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="a0e85-157">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-157">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="a0e85-158">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="a0e85-158">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="a0e85-159">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="a0e85-159">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-160">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-160">AppService</span></span>
* <span data-ttu-id="a0e85-161">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="a0e85-161">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="a0e85-162">Correction du bogue où les emplacements ne fonctionnaient pas pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-162">Fixed bug where slots didn't work for</span></span> `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a><span data-ttu-id="a0e85-163">Service BOT</span><span class="sxs-lookup"><span data-stu-id="a0e85-163">BOT Service</span></span>
* <span data-ttu-id="a0e85-164">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via</span><span class="sxs-lookup"><span data-stu-id="a0e85-164">Added `bot prepare-deploy` to prepare for deploying bots via</span></span> `webapp`
* <span data-ttu-id="a0e85-165">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="a0e85-165">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="a0e85-166">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="a0e85-166">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="a0e85-167">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a0e85-167">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="a0e85-168">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-168">CDN</span></span>
* <span data-ttu-id="a0e85-169">Ajout de la prise en charge de `--no-wait` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-169">Added support for `--no-wait` to</span></span> `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* <span data-ttu-id="a0e85-170">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-170">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="a0e85-171">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="a0e85-171">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a0e85-172">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="a0e85-172">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-173">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a0e85-173">Cosmosdb</span></span>
* <span data-ttu-id="a0e85-174">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="a0e85-174">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="a0e85-175">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0e85-175">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-176">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-176">Interactive</span></span>
* <span data-ttu-id="a0e85-177">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="a0e85-177">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-178">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-178">Monitor</span></span>
* <span data-ttu-id="a0e85-179">Changement apporté pour autoriser la valeur de dimension `*` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-179">Changed to allow dimension value `*` for</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="a0e85-180">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-180">Network</span></span>
* <span data-ttu-id="a0e85-181">Ajout du groupe de commandes `rewrite-rule` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-181">Added `rewrite-rule` command group to</span></span> `application-gateway`

### <a name="profile"></a><span data-ttu-id="a0e85-182">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-182">Profile</span></span>
* <span data-ttu-id="a0e85-183">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-183">Added tenant level account support for managed service identity to</span></span> `login`

### <a name="postgres"></a><span data-ttu-id="a0e85-184">Postgres</span><span class="sxs-lookup"><span data-stu-id="a0e85-184">Postgres</span></span> 
* <span data-ttu-id="a0e85-185">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="a0e85-185">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="a0e85-186">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="a0e85-186">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-187">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-187">Resource</span></span>
* <span data-ttu-id="a0e85-188">Amélioration de la sortie de table pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-188">Improved table output for</span></span> `deployment [create|list|show]`
* <span data-ttu-id="a0e85-189">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="a0e85-189">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="a0e85-190">Graph</span><span class="sxs-lookup"><span data-stu-id="a0e85-190">Graph</span></span>
* <span data-ttu-id="a0e85-191">Ajout de la prise en charge de `--end-date` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-191">Added support for `--end-date` to</span></span> `ad [app|sp] credential reset`
* <span data-ttu-id="a0e85-192">Ajout de la prise en charge de l’ajout d’autorisations avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-192">Added support to add permissions with</span></span> `ad app permission add`
* <span data-ttu-id="a0e85-193">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="a0e85-193">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="a0e85-194">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-194">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="a0e85-195">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="a0e85-195">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-196">storage</span><span class="sxs-lookup"><span data-stu-id="a0e85-196">storage</span></span>
* <span data-ttu-id="a0e85-197">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="a0e85-197">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="a0e85-198">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="a0e85-198">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="a0e85-199">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="a0e85-199">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="a0e85-200">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="a0e85-200">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-201">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-201">VM</span></span>
* <span data-ttu-id="a0e85-202">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-202">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="a0e85-203">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-203">March 12, 2019</span></span>

<span data-ttu-id="a0e85-204">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="a0e85-204">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-205">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-205">Core</span></span>

* <span data-ttu-id="a0e85-206">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="a0e85-206">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-207">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-207">ACR</span></span>

* <span data-ttu-id="a0e85-208">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="a0e85-208">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-209">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-209">ACS</span></span>

* <span data-ttu-id="a0e85-210">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="a0e85-210">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="a0e85-211">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-211">AppService</span></span>

* <span data-ttu-id="a0e85-212">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="a0e85-212">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="a0e85-213">Suppression d’une instruction print erronée pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-213">Removed erroneous print statement for</span></span> `webapp auth update`
* <span data-ttu-id="a0e85-214">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-214">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="a0e85-215">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-215">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="a0e85-216">Botservice</span><span class="sxs-lookup"><span data-stu-id="a0e85-216">Botservice</span></span>

* <span data-ttu-id="a0e85-217">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a0e85-217">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a0e85-218">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="a0e85-218">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a0e85-219">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de</span><span class="sxs-lookup"><span data-stu-id="a0e85-219">Removed single quotes from `bot publish` command output at end of</span></span> `bot create`
* <span data-ttu-id="a0e85-220">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="a0e85-220">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-221">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-221">Container</span></span>

* <span data-ttu-id="a0e85-222">Ajout de l’argument `--no-wait` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-222">Added `--no-wait` argument to</span></span> `container [start|restart]`

### <a name="eventhub"></a><span data-ttu-id="a0e85-223">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a0e85-223">EventHub</span></span>

* <span data-ttu-id="a0e85-224">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="a0e85-224">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="a0e85-225">Rechercher</span><span class="sxs-lookup"><span data-stu-id="a0e85-225">Find</span></span>

* <span data-ttu-id="a0e85-226">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a0e85-226">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a0e85-227">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0e85-227">HDInsight</span></span>

* <span data-ttu-id="a0e85-228">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="a0e85-228">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-229">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-229">Network</span></span>

* <span data-ttu-id="a0e85-230">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="a0e85-230">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a0e85-231">Rdbms</span></span>

* <span data-ttu-id="a0e85-232">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="a0e85-232">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-233">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-233">Role</span></span>

* <span data-ttu-id="a0e85-234">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="a0e85-234">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="a0e85-235">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="a0e85-235">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0e85-236">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0e85-236">Service Fabric</span></span>

* <span data-ttu-id="a0e85-237">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="a0e85-237">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="a0e85-238">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-238">February 26, 2019</span></span>

<span data-ttu-id="a0e85-239">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="a0e85-239">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-240">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-240">Core</span></span>

* <span data-ttu-id="a0e85-241">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="a0e85-241">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-242">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-242">ACR</span></span>

* <span data-ttu-id="a0e85-243">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-243">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="a0e85-244">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="a0e85-244">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-245">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-245">ACS</span></span>

* <span data-ttu-id="a0e85-246">Ajout de l’option `--listen-address` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-246">Added `--listen-address` option to</span></span> `aks port-forward`

### <a name="appservice"></a><span data-ttu-id="a0e85-247">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-247">AppService</span></span>

* <span data-ttu-id="a0e85-248">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="a0e85-248">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-249">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-249">Batch</span></span>
* <span data-ttu-id="a0e85-250">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="a0e85-250">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="a0e85-251">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="a0e85-251">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="a0e85-252">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="a0e85-252">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="a0e85-253">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="a0e85-253">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="a0e85-254">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="a0e85-254">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="a0e85-255">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="a0e85-255">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-256">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-256">CosmosDB</span></span>

* <span data-ttu-id="a0e85-257">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0e85-257">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="a0e85-258">Kusto</span><span class="sxs-lookup"><span data-stu-id="a0e85-258">Kusto</span></span>

* <span data-ttu-id="a0e85-259">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="a0e85-259">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-260">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-260">Network</span></span>

* <span data-ttu-id="a0e85-261">Ajout de l’argument `--express-route-gateway-bypass` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-261">Added `--express-route-gateway-bypass` argument to</span></span> `vpn-connection [create|update]`
* <span data-ttu-id="a0e85-262">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="a0e85-262">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="a0e85-263">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="a0e85-263">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="a0e85-264">Ajout de l’argument `--legacy-mode` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-264">Added argument `--legacy-mode` to</span></span> `express-route peering [create|update]` 
* <span data-ttu-id="a0e85-265">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-265">Added arguments `--allow-classic-operations` and `--express-route-port` to</span></span> `express-route [create|update]`
* <span data-ttu-id="a0e85-266">Ajout de l’argument `--gateway-default-site` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-266">Added `--gateway-default-site` argument to</span></span> `vnet-gateway [create|update]`
* <span data-ttu-id="a0e85-267">Ajout des commandes `ipsec-policy` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-267">Added `ipsec-policy` commands to</span></span> `vnet-gateway`

### <a name="resource"></a><span data-ttu-id="a0e85-268">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-268">Resource</span></span>

* <span data-ttu-id="a0e85-269">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-269">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="a0e85-270">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur</span><span class="sxs-lookup"><span data-stu-id="a0e85-270">Added support for URI-based parameters file to</span></span> `policy assignment create`
* <span data-ttu-id="a0e85-271">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur</span><span class="sxs-lookup"><span data-stu-id="a0e85-271">Added support for URI-based parameters and definitions to</span></span> `policy set-definition update`
* <span data-ttu-id="a0e85-272">Correction de la gestion des paramètres et des règles pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-272">Fixed handling of parameters and rules for</span></span> `policy definition update`
* <span data-ttu-id="a0e85-273">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-273">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-274">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-274">Role</span></span>

* <span data-ttu-id="a0e85-275">Ajout de la prise en charge des rôles d’application sur</span><span class="sxs-lookup"><span data-stu-id="a0e85-275">Added support for app roles to</span></span> `ad app [create|update]`

### <a name="vm"></a><span data-ttu-id="a0e85-276">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-276">VM</span></span>

* <span data-ttu-id="a0e85-277">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="a0e85-277">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="a0e85-278">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-278">February 12, 2019</span></span>

<span data-ttu-id="a0e85-279">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="a0e85-279">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-280">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-280">Core</span></span>

* `az --version` <span data-ttu-id="a0e85-281">affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="a0e85-281">now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="a0e85-282">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="a0e85-282">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-283">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-283">ACR</span></span>
* <span data-ttu-id="a0e85-284">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="a0e85-284">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="a0e85-285">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-285">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from</span></span> `acr repository delete`

### <a name="acs"></a><span data-ttu-id="a0e85-286">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-286">ACS</span></span>
* <span data-ttu-id="a0e85-287">Ajout de la prise en charge des noms qui ne respectent pas la casse à</span><span class="sxs-lookup"><span data-stu-id="a0e85-287">Added support for case-insensitive names to</span></span> `aks [enable-addons|disable-addons]`
* <span data-ttu-id="a0e85-288">Ajout de la prise en charge de la mise à jour d’Azure Active Directory avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-288">Added support for Azure Active Directory updating operation using</span></span> `aks update-credentials --reset-aad`
* <span data-ttu-id="a0e85-289">Ajout d’une clarification indiquant que `--output` est ignoré pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-289">Added clarification that `--output` is ignored for</span></span> `aks get-credentials`

### <a name="ams"></a><span data-ttu-id="a0e85-290">AMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-290">AMS</span></span>
* <span data-ttu-id="a0e85-291">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="a0e85-291">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="a0e85-292">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="a0e85-292">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-293">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-293">Appservice</span></span>
* <span data-ttu-id="a0e85-294">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-294">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="a0e85-295">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="a0e85-295">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="a0e85-296">Amélioration de l’aide pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-296">Improved help for</span></span> `appservice-plan-update`
* <span data-ttu-id="a0e85-297">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="a0e85-297">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="a0e85-298">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="a0e85-298">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="a0e85-299">Botservice</span><span class="sxs-lookup"><span data-stu-id="a0e85-299">Botservice</span></span>
* <span data-ttu-id="a0e85-300">Amélioration de l’expérience utilisateur pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-300">Improved UX for</span></span> `bot publish`
* <span data-ttu-id="a0e85-301">Ajout d’un avertissement pour les délais d’expiration quand `npm install` est exécuté durant</span><span class="sxs-lookup"><span data-stu-id="a0e85-301">Added warning for timeouts when running `npm install` during</span></span> `az bot publish`
* <span data-ttu-id="a0e85-302">Suppression du caractère non valide `.` de `--name` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-302">Removed invalid char `.` from `--name`  in</span></span> `az bot create`
* <span data-ttu-id="a0e85-303">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="a0e85-303">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="a0e85-304">[[DÉPRÉCIÉ]] Dépréciation de l’argument `--proj-name` en faveur de</span><span class="sxs-lookup"><span data-stu-id="a0e85-304">[DEPRECATED] Deprecated `--proj-name` argument in favor of</span></span> `--proj-file-path`
* <span data-ttu-id="a0e85-305">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="a0e85-305">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="a0e85-306">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="a0e85-306">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="a0e85-307">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="a0e85-307">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="a0e85-308">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="a0e85-308">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="a0e85-309">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="a0e85-309">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="a0e85-310">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a0e85-310">Key Vault</span></span>
* <span data-ttu-id="a0e85-311">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient</span><span class="sxs-lookup"><span data-stu-id="a0e85-311">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using</span></span> `--id`

### <a name="monitor"></a><span data-ttu-id="a0e85-312">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-312">Monitor</span></span>
* <span data-ttu-id="a0e85-313">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension</span><span class="sxs-lookup"><span data-stu-id="a0e85-313">Changed `monitor metrics alert [create|update]` to allow dimension value</span></span> `*`

### <a name="network"></a><span data-ttu-id="a0e85-314">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-314">Network</span></span>
* <span data-ttu-id="a0e85-315">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="a0e85-315">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="a0e85-316">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a0e85-316">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="a0e85-317">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="a0e85-317">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="a0e85-318">Ajout de `--idle-timeout` et `--floating-ip` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-318">Added `--idle-timeout` and `--floating-ip` to</span></span> `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a><span data-ttu-id="a0e85-319">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a0e85-319">Policy Insights</span></span>
* <span data-ttu-id="a0e85-320">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="a0e85-320">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-321">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-321">RDBMS</span></span>
* <span data-ttu-id="a0e85-322">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-322">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="a0e85-323">Redis</span><span class="sxs-lookup"><span data-stu-id="a0e85-323">Redis</span></span>
* <span data-ttu-id="a0e85-324">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="a0e85-324">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="a0e85-325">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="a0e85-325">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="a0e85-326">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="a0e85-326">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="a0e85-327">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="a0e85-327">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="a0e85-328">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="a0e85-328">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="a0e85-329">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="a0e85-329">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="a0e85-330">[[DÉPRÉCIÉ]] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="a0e85-330">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-331">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-331">Role</span></span>
* <span data-ttu-id="a0e85-332">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="a0e85-332">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="a0e85-333">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-333">SQL VM</span></span>
* <span data-ttu-id="a0e85-334">[[DÉPRÉCIÉ]] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="a0e85-334">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-335">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-335">VM</span></span>
* <span data-ttu-id="a0e85-336">Changement apporté à `vm list-skus` pour autoriser l’utilisation de `--all` à la place de</span><span class="sxs-lookup"><span data-stu-id="a0e85-336">Changed `vm list-skus` to allow use of `--all` in place of</span></span> `--all true`
* <span data-ttu-id="a0e85-337">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-337">Added</span></span> `vmss run-command [invoke | list | show]`
* <span data-ttu-id="a0e85-338">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="a0e85-338">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="a0e85-339">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="a0e85-339">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="a0e85-340">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-340">January 31, 2019</span></span>

<span data-ttu-id="a0e85-341">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="a0e85-341">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-342">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-342">Core</span></span>

* <span data-ttu-id="a0e85-343">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="a0e85-343">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="a0e85-344">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-344">January 28, 2019</span></span>

<span data-ttu-id="a0e85-345">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="a0e85-345">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-346">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-346">ACR</span></span>
* <span data-ttu-id="a0e85-347">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="a0e85-347">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-348">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-348">ACS</span></span>
* <span data-ttu-id="a0e85-349">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="a0e85-349">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a0e85-350">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="a0e85-350">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="a0e85-351">Ajout de la prise en charge des mises à jour du principal de service avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-351">Added support for service principal updates operation with</span></span> `aks update-credentials -reset-service-principal`

### <a name="ams"></a><span data-ttu-id="a0e85-352">AMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-352">AMS</span></span>
* <span data-ttu-id="a0e85-353">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-353">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to</span></span> `ams asset list-streaming-locators`
* <span data-ttu-id="a0e85-354">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-354">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to</span></span> `ams streaming-locator list-content-keys`

### <a name="appservice"></a><span data-ttu-id="a0e85-355">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-355">Appservice</span></span>
* <span data-ttu-id="a0e85-356">Ajout de la prise en charge d’Application Insights sur</span><span class="sxs-lookup"><span data-stu-id="a0e85-356">Added support for app insights on</span></span> `functionapp create`
* <span data-ttu-id="a0e85-357">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="a0e85-357">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="a0e85-358">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="a0e85-358">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-359">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-359">Container</span></span>
* <span data-ttu-id="a0e85-360">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="a0e85-360">Added `container start` command</span></span>
* <span data-ttu-id="a0e85-361">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-361">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a0e85-362">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a0e85-362">EventGrid</span></span>
* <span data-ttu-id="a0e85-363">Ajout du paramètre `--deadletter-endpoint` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-363">Added `--deadletter-endpoint` parameter to</span></span> `event-subscription [create|update]`
* <span data-ttu-id="a0e85-364">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="a0e85-364">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="a0e85-365">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="a0e85-365">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="a0e85-366">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="a0e85-366">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="a0e85-367">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="a0e85-367">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a0e85-368">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0e85-368">HDInsight</span></span>
* <span data-ttu-id="a0e85-369">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-369">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from</span></span> `hdinsight [application] create`
* <span data-ttu-id="a0e85-370">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="a0e85-370">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="a0e85-371">Ajout des paramètres `--vnet-name` et `--subnet-name` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-371">Added `--vnet-name` and `--subnet-name` parameters to</span></span> `hdinsight create`
* <span data-ttu-id="a0e85-372">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à</span><span class="sxs-lookup"><span data-stu-id="a0e85-372">Added support for Enterprise Security Package and disk encryption to</span></span> `hdinsight create` 
* <span data-ttu-id="a0e85-373">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="a0e85-373">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="a0e85-374">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-374">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-375">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-375">IoT</span></span>
* <span data-ttu-id="a0e85-376">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="a0e85-376">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="a0e85-377">Kusto</span><span class="sxs-lookup"><span data-stu-id="a0e85-377">Kusto</span></span>
* <span data-ttu-id="a0e85-378">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-378">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-379">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-379">Monitor</span></span>
* <span data-ttu-id="a0e85-380">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-380">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="a0e85-381">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-381">Profile</span></span>
* <span data-ttu-id="a0e85-382">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-382">Enable tenant level account for managed service identity for</span></span> `login`

### <a name="network"></a><span data-ttu-id="a0e85-383">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-383">Network</span></span>
* <span data-ttu-id="a0e85-384">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="a0e85-384">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="a0e85-385">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="a0e85-385">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-386">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-386">Resource</span></span>
* <span data-ttu-id="a0e85-387">Ajout de la prise en charge du fichier de paramètres d’URI à</span><span class="sxs-lookup"><span data-stu-id="a0e85-387">Added support for URI parameters file to</span></span> `group deployment create`
* <span data-ttu-id="a0e85-388">Ajout de la prise en charge de la fonctionnalité Managed Service Identity à</span><span class="sxs-lookup"><span data-stu-id="a0e85-388">Added support for managed identity to</span></span> `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a><span data-ttu-id="a0e85-389">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-389">SQL Virtual Machine</span></span>
* <span data-ttu-id="a0e85-390">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-390">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-391">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-391">Storage</span></span>
* <span data-ttu-id="a0e85-392">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="a0e85-392">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="a0e85-393">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="a0e85-393">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-394">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-394">VM</span></span>
* <span data-ttu-id="a0e85-395">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="a0e85-395">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="a0e85-396">Ajout de l’indicateur `--force` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-396">Added `--force` flag to</span></span> `vm encryption enable`

## <a name="january-15-2019"></a><span data-ttu-id="a0e85-397">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="a0e85-397">January 15, 2019</span></span>

<span data-ttu-id="a0e85-398">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="a0e85-398">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-399">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-399">ACR</span></span>
* <span data-ttu-id="a0e85-400">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-400">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="a0e85-401">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="a0e85-401">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="a0e85-402">[[DÉPRÉCIÉ]] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-402">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="a0e85-403">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-403">ACS</span></span>
* <span data-ttu-id="a0e85-404">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="a0e85-404">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-405">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-405">Appservice</span></span>
* <span data-ttu-id="a0e85-406">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="a0e85-406">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="a0e85-407">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-407">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="a0e85-408">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="a0e85-408">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="a0e85-409">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="a0e85-409">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="a0e85-410">Botservice</span><span class="sxs-lookup"><span data-stu-id="a0e85-410">Botservice</span></span>
* <span data-ttu-id="a0e85-411">Ajout de mises à jour de l’état de déploiement à</span><span class="sxs-lookup"><span data-stu-id="a0e85-411">Added deployment status updates to</span></span> `bot create`

### <a name="configure"></a><span data-ttu-id="a0e85-412">Configuration</span><span class="sxs-lookup"><span data-stu-id="a0e85-412">Configure</span></span>
* <span data-ttu-id="a0e85-413">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="a0e85-413">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-414">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-414">CosmosDB</span></span>
* <span data-ttu-id="a0e85-415">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="a0e85-415">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a0e85-416">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0e85-416">HDInsight</span></span>
* <span data-ttu-id="a0e85-417">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="a0e85-417">Added commands for managing applications</span></span>
* <span data-ttu-id="a0e85-418">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="a0e85-418">Added commands for managing script actions</span></span>
* <span data-ttu-id="a0e85-419">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="a0e85-419">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="a0e85-420">Ajout de la prise en charge permettant de lister l’utilisation régionale à</span><span class="sxs-lookup"><span data-stu-id="a0e85-420">Added support to list regional usage to</span></span> `hdinsight list-usage`
* <span data-ttu-id="a0e85-421">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-421">[BREAKING CHANGE] Removed default cluster type from</span></span> `hdinsight create`

### <a name="network"></a><span data-ttu-id="a0e85-422">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-422">Network</span></span>
* <span data-ttu-id="a0e85-423">Ajout des arguments `--custom-headers` et `--status-code-ranges` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-423">Added `--custom-headers` and `--status-code-ranges` arguments to</span></span> `traffic-manager profile [create|update]`
* <span data-ttu-id="a0e85-424">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="a0e85-424">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="a0e85-425">Ajout des arguments `--custom-headers` et `--subnets` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-425">Added `--custom-headers` and `--subnets` arguments to</span></span> `traffic-manager endpoint [create|update]`  
* <span data-ttu-id="a0e85-426">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="a0e85-426">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-427">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-427">Role</span></span>
* <span data-ttu-id="a0e85-428">[[DÉPRÉCIÉ]] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-428">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="a0e85-429">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="a0e85-429">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="a0e85-430">Sécurité</span><span class="sxs-lookup"><span data-stu-id="a0e85-430">Security</span></span>
* <span data-ttu-id="a0e85-431">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-431">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-432">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-432">Storage</span></span>
* <span data-ttu-id="a0e85-433">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="a0e85-433">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="a0e85-434">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="a0e85-434">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="a0e85-435">Ajout du paramètre `--marker` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-435">Added `--marker` parameter to</span></span> `storage [blob|file|container|share] list`
* <span data-ttu-id="a0e85-436">Ajout du marqueur de journal de la page suivante à STDERR pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-436">Added log marker for next page to STDERR for</span></span> `storage [blob|file|container|share] list` 
* <span data-ttu-id="a0e85-437">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-437">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-438">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-438">VM</span></span>
* <span data-ttu-id="a0e85-439">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="a0e85-439">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="a0e85-440">Ajout de la prise en charge du référencement d’images entre locataires à</span><span class="sxs-lookup"><span data-stu-id="a0e85-440">Added support for cross tenant image referencing to</span></span> `[vm|vmss] create`
* <span data-ttu-id="a0e85-441">Résolution d’un bogue lié à la configuration par défaut dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-441">Fixed bug with default configuration in</span></span> `vm diagnostics get-default-config --windows-os`
* <span data-ttu-id="a0e85-442">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-442">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="a0e85-443">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-443">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="a0e85-444">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="a0e85-444">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="a0e85-445">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-445">December 20, 2018</span></span>

<span data-ttu-id="a0e85-446">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="a0e85-446">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="a0e85-447">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-447">Appservice</span></span>
* <span data-ttu-id="a0e85-448">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a0e85-448">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="a0e85-449">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="a0e85-449">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="a0e85-450">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-450">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a0e85-451">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a0e85-451">IoTCentral</span></span>
* <span data-ttu-id="a0e85-452">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="a0e85-452">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-453">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-453">Role</span></span>
* <span data-ttu-id="a0e85-454">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="a0e85-454">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-455">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-455">SQL</span></span>
* <span data-ttu-id="a0e85-456">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="a0e85-456">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-457">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-457">VM</span></span>
* <span data-ttu-id="a0e85-458">Ajout du paramètre `---os-type` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-458">Added `---os-type` parameter to</span></span> `disk create`

## <a name="december-18-2018"></a><span data-ttu-id="a0e85-459">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-459">December 18, 2018</span></span>

<span data-ttu-id="a0e85-460">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="a0e85-460">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="a0e85-461">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-461">ACR</span></span>
* <span data-ttu-id="a0e85-462">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="a0e85-462">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="a0e85-463">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="a0e85-463">Condensed the table layout for task list</span></span>
* <span data-ttu-id="a0e85-464">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a0e85-464">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-465">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-465">ACS</span></span>
* <span data-ttu-id="a0e85-466">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="a0e85-466">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a0e85-467">Suppression de « (PREVIEW) » dans les arguments AAD pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-467">Removed "(PREVIEW)" from AAD arguments to</span></span> `aks create`
* <span data-ttu-id="a0e85-468">[[DÉPRÉCIÉ]] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-468">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="a0e85-469">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="a0e85-469">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="a0e85-470">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-470">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="a0e85-471">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="a0e85-471">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-472">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-472">Appservice</span></span>
* <span data-ttu-id="a0e85-473">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="a0e85-473">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="a0e85-474">Botservice</span><span class="sxs-lookup"><span data-stu-id="a0e85-474">Botservice</span></span>
* <span data-ttu-id="a0e85-475">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de</span><span class="sxs-lookup"><span data-stu-id="a0e85-475">Added support for `.bot` file parsing when calling</span></span> `bot show`
* <span data-ttu-id="a0e85-476">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="a0e85-476">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="a0e85-477">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="a0e85-477">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="a0e85-478">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="a0e85-478">Reduced Kudu network calls</span></span>
* <span data-ttu-id="a0e85-479">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="a0e85-479">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="a0e85-480">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-480">Consumption</span></span>
* <span data-ttu-id="a0e85-481">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="a0e85-481">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-482">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-482">CosmosDB</span></span>
* <span data-ttu-id="a0e85-483">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="a0e85-483">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="a0e85-484">Cartes</span><span class="sxs-lookup"><span data-stu-id="a0e85-484">Maps</span></span>
* <span data-ttu-id="a0e85-485">Ajout de la prise en charge de la référence SKU S1 pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-485">Added support for the S1 SKU to</span></span> `maps account [create|update]`

### <a name="network"></a><span data-ttu-id="a0e85-486">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-486">Network</span></span>
* <span data-ttu-id="a0e85-487">Ajout de la prise en charge de `--format` et `--log-version` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-487">Added support for `--format` and `--log-version` to</span></span> `watcher flow-log configure`
* <span data-ttu-id="a0e85-488">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-488">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-489">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-489">Resource</span></span>
* <span data-ttu-id="a0e85-490">Correction du traitement du paramètre de portée (scope) pour les groupes d’administration dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-490">Fixed handling of scope parameter for management groups in</span></span> `policy assignment [create|list|delete|show|update]` 
* <span data-ttu-id="a0e85-491">Ajout d’une nouvelle commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-491">Added new command</span></span> `resource wait`

### <a name="storage"></a><span data-ttu-id="a0e85-492">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-492">Storage</span></span>
*  <span data-ttu-id="a0e85-493">Ajout de la possibilité de mettre à jour la version du schéma de journal pour les services de stockage dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-493">Added ability to update log schema version for storage services in</span></span> `storage logging update`

### <a name="vm"></a><span data-ttu-id="a0e85-494">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-494">VM</span></span>
* <span data-ttu-id="a0e85-495">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="a0e85-495">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="a0e85-496">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-496">December 4, 2018</span></span>

<span data-ttu-id="a0e85-497">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="a0e85-497">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="a0e85-498">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-498">Core</span></span>
* <span data-ttu-id="a0e85-499">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="a0e85-499">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="a0e85-500">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="a0e85-500">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-501">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-501">Appservice</span></span>
* <span data-ttu-id="a0e85-502">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="a0e85-502">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="a0e85-503">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="a0e85-503">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-504">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-504">Network</span></span>
* <span data-ttu-id="a0e85-505">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="a0e85-505">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-506">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-506">Role</span></span>
* <span data-ttu-id="a0e85-507">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="a0e85-507">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="a0e85-508">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-508">VM</span></span>
* <span data-ttu-id="a0e85-509">[[DÉPRÉCIÉ]] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="a0e85-509">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="a0e85-510">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="a0e85-510">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="a0e85-511">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="a0e85-511">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="a0e85-512">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="a0e85-512">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="a0e85-513">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-513">November 20, 2018</span></span>

<span data-ttu-id="a0e85-514">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="a0e85-514">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="a0e85-515">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-515">Core</span></span>
* <span data-ttu-id="a0e85-516">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="a0e85-516">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-517">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-517">ACR</span></span>
* <span data-ttu-id="a0e85-518">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="a0e85-518">Added context token to task step</span></span>
* <span data-ttu-id="a0e85-519">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="a0e85-519">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="a0e85-520">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="a0e85-520">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-521">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-521">Appservice</span></span>
* <span data-ttu-id="a0e85-522">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="a0e85-522">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="a0e85-523">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-523">Updated the default `node_version`.</span></span> <span data-ttu-id="a0e85-524">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="a0e85-524">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="a0e85-525">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-525">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="a0e85-526">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="a0e85-526">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a0e85-527">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a0e85-527">IotCentral</span></span>
* <span data-ttu-id="a0e85-528">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="a0e85-528">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-529">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-529">KeyVault</span></span>
* <span data-ttu-id="a0e85-530">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="a0e85-530">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-531">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-531">Network</span></span>
* <span data-ttu-id="a0e85-532">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="a0e85-532">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="a0e85-533">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="a0e85-533">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="a0e85-534">Ajout de `--zones` pour la prise en charge de zone de disponibilité à</span><span class="sxs-lookup"><span data-stu-id="a0e85-534">Added `--zones` for availability zone support to</span></span> `application-gateway create` 
* <span data-ttu-id="a0e85-535">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-535">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to</span></span> `application-gateway waf-config set`

### <a name="rdbms"></a><span data-ttu-id="a0e85-536">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a0e85-536">Rdbms</span></span>
* <span data-ttu-id="a0e85-537">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="a0e85-537">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="a0e85-538">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="a0e85-538">Rbac</span></span>
* <span data-ttu-id="a0e85-539">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-539">Fixed an issue with attempting to update immutable credentials in</span></span> `ad app update`
* <span data-ttu-id="a0e85-540">Ajout d’avertissements de sortie pour indiquer les prochains changements cassants pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-540">Added output warnings to communicate breaking changes in the near future for</span></span> `ad [app|sp] list` 

### <a name="storage"></a><span data-ttu-id="a0e85-541">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-541">Storage</span></span>
* <span data-ttu-id="a0e85-542">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-542">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="a0e85-543">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-543">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="a0e85-544">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="a0e85-544">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="a0e85-545">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="a0e85-545">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-546">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-546">VM</span></span>
* <span data-ttu-id="a0e85-547">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="a0e85-547">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="a0e85-548">Remplacement des paramètres de nom de version `sig image-version` par</span><span class="sxs-lookup"><span data-stu-id="a0e85-548">Changed version name parameters to `sig image-version` to be</span></span> `--image-version -e`
* <span data-ttu-id="a0e85-549">Valeur `sig image-version` dépréciée pour l’argument `--image-version-name`, remplacée par</span><span class="sxs-lookup"><span data-stu-id="a0e85-549">Deprecated `sig image-version` argument `--image-version-name`, replaced by</span></span> `--image-version`
* <span data-ttu-id="a0e85-550">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-550">Added support to use local OS disk to</span></span> `[vm|vmss] create --ephemeral-os-disk`
* <span data-ttu-id="a0e85-551">Ajout de la prise en charge de `--no-wait` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-551">Added support for `--no-wait` to</span></span> `snapshot create/update`
* <span data-ttu-id="a0e85-552">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="a0e85-552">Added `snapshot wait` command</span></span>
* <span data-ttu-id="a0e85-553">Ajout de la prise en charge pour utiliser le nom d’instance avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-553">Added support for using instance name with</span></span> `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a><span data-ttu-id="a0e85-554">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-554">November 6, 2018</span></span>

<span data-ttu-id="a0e85-555">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="a0e85-555">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-556">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-556">Core</span></span>
* <span data-ttu-id="a0e85-557">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="a0e85-557">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-558">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-558">ACR</span></span>
* <span data-ttu-id="a0e85-559">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="a0e85-559">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="a0e85-560">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="a0e85-560">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-561">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-561">ACS</span></span>
* <span data-ttu-id="a0e85-562">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-562">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="a0e85-563">Advisor</span><span class="sxs-lookup"><span data-stu-id="a0e85-563">Advisor</span></span>
* <span data-ttu-id="a0e85-564">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="a0e85-564">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="a0e85-565">AMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-565">AMS</span></span>
* <span data-ttu-id="a0e85-566">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-566">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="a0e85-567">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-567">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="a0e85-568">Ajout de la prise en charge des paramètres de chiffrement dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-568">Added encryption parameters support to</span></span> `ams streaming-policy create`
* <span data-ttu-id="a0e85-569">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="a0e85-569">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="a0e85-570">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="a0e85-570">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="a0e85-571">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="a0e85-571">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="a0e85-572">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="a0e85-572">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="a0e85-573">[CHANGEMENT CASSANT] Remplacement de la commande `ams streaming locator` par</span><span class="sxs-lookup"><span data-stu-id="a0e85-573">[BREAKING CHANGE] Replaced `ams streaming locator` command with</span></span> `ams streaming-locator`
* <span data-ttu-id="a0e85-574">[CHANGEMENT CASSANT] Mise à jour de l’argument `--content-keys` de</span><span class="sxs-lookup"><span data-stu-id="a0e85-574">[BREAKING CHANGE] Updated `--content-keys` argument of</span></span> `ams streaming locator`
* <span data-ttu-id="a0e85-575">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="a0e85-575">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="a0e85-576">[CHANGEMENT CASSANT] Remplacement de la commande `ams streaming policy` par</span><span class="sxs-lookup"><span data-stu-id="a0e85-576">[BREAKING CHANGE] Replaced `ams streaming policy` command with</span></span> `ams streaming-policy`
* <span data-ttu-id="a0e85-577">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-577">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="a0e85-578">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="a0e85-578">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="a0e85-579">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="a0e85-579">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="a0e85-580">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-580">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="a0e85-581">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="a0e85-581">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="a0e85-582">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="a0e85-582">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-583">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-583">AppService</span></span>
* <span data-ttu-id="a0e85-584">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="a0e85-584">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="a0e85-585">Configuration</span><span class="sxs-lookup"><span data-stu-id="a0e85-585">Configure</span></span>
* <span data-ttu-id="a0e85-586">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="a0e85-586">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-587">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-587">Container</span></span>
* <span data-ttu-id="a0e85-588">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="a0e85-588">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="a0e85-589">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a0e85-589">EventHub</span></span>
* <span data-ttu-id="a0e85-590">Ajout de l’indicateur `--enable-kafka` pour prendre en charge Kafka dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-590">Added `--enable-kafka` flag to support Kafka in</span></span> `eventhub namespace [create|update]`

### <a name="interactive"></a><span data-ttu-id="a0e85-591">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-591">Interactive</span></span>
* <span data-ttu-id="a0e85-592">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="a0e85-592">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-593">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-593">Monitor</span></span>
* <span data-ttu-id="a0e85-594">Ajout de la prise en charge des noms de métriques incluant les caractères barre oblique (/) et point (.) à `--condition` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-594">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="a0e85-595">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-595">Network</span></span>
* <span data-ttu-id="a0e85-596">Dépréciation des noms de commande `network interface-endpoint` en faveur de</span><span class="sxs-lookup"><span data-stu-id="a0e85-596">Deprecated `network interface-endpoint` command names in favor of</span></span> `network private-endpoint`
* <span data-ttu-id="a0e85-597">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-597">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="a0e85-598">Correction du problème où `--ip-tags` ne fonctionnait pas correctement avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-598">Fixed issue where `--ip-tags` did not work correctly with</span></span> `public-ip create` 

### <a name="profile"></a><span data-ttu-id="a0e85-599">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-599">Profile</span></span>
* <span data-ttu-id="a0e85-600">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="a0e85-600">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-601">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-601">RDBMS</span></span>
* <span data-ttu-id="a0e85-602">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="a0e85-602">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-603">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-603">Resource</span></span>
* <span data-ttu-id="a0e85-604">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="a0e85-604">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-605">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-605">Role</span></span>
* <span data-ttu-id="a0e85-606">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="a0e85-606">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="a0e85-607">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="a0e85-607">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="a0e85-608">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="a0e85-608">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-609">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-609">Storage</span></span>
* <span data-ttu-id="a0e85-610">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="a0e85-610">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-611">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-611">VM</span></span>
* <span data-ttu-id="a0e85-612">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="a0e85-612">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="a0e85-613">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-613">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="a0e85-614">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="a0e85-614">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="a0e85-615">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="a0e85-615">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="a0e85-616">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="a0e85-616">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="a0e85-617">Amélioration de la validation de l’argument pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-617">Improved argument validation for</span></span> `vm create --image`

## <a name="october-23-2018"></a><span data-ttu-id="a0e85-618">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-618">October 23, 2018</span></span>

<span data-ttu-id="a0e85-619">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="a0e85-619">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-620">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-620">Core</span></span>
* <span data-ttu-id="a0e85-621">Correction du problème avec `--ids` où `--subscription` était prioritaire sur l’abonnement dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-621">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in</span></span> `--ids`
* <span data-ttu-id="a0e85-622">Ajout d’avertissements explicites quand les paramètres sont ignorés par</span><span class="sxs-lookup"><span data-stu-id="a0e85-622">Added explicit warnings when parameters would be ignored by use of</span></span> `--ids`

### <a name="acr"></a><span data-ttu-id="a0e85-623">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-623">ACR</span></span>
* <span data-ttu-id="a0e85-624">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="a0e85-624">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="a0e85-625">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-625">CDN</span></span>
* <span data-ttu-id="a0e85-626">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="a0e85-626">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a0e85-627">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="a0e85-627">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-628">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-628">Container</span></span>
* <span data-ttu-id="a0e85-629">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="a0e85-629">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="a0e85-630">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-630">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="a0e85-631">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="a0e85-631">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="a0e85-632">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-632">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="a0e85-633">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="a0e85-633">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="a0e85-634">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="a0e85-634">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="a0e85-635">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-635">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-636">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-636">CosmosDB</span></span>
* <span data-ttu-id="a0e85-637">Ajout de la prise en charge de `--enable-multiple-write-locations` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-637">Added `--enable-multiple-write-locations` support to</span></span> `cosmosdb create`

### <a name="interactive"></a><span data-ttu-id="a0e85-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-638">Interactive</span></span>
* <span data-ttu-id="a0e85-639">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="a0e85-639">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="a0e85-640">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a0e85-640">IoT Central</span></span>
* <span data-ttu-id="a0e85-641">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="a0e85-641">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="a0e85-642">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="a0e85-642">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-643">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-643">Monitor</span></span>
* <span data-ttu-id="a0e85-644">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="a0e85-644">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="a0e85-645">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-645">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="a0e85-646">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="a0e85-646">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a0e85-647">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="a0e85-647">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="a0e85-648">Ajout de `--namespace` comme alias pour l’option dépréciée</span><span class="sxs-lookup"><span data-stu-id="a0e85-648">Added `--namespace` as alias for deprecated option</span></span> `--resource-provider`
  * <span data-ttu-id="a0e85-649">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="a0e85-649">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="a0e85-650">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="a0e85-650">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="a0e85-651">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="a0e85-651">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a0e85-652">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="a0e85-652">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="a0e85-653">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-653">Improved validation for `--event-hub` and `--event-hub-rule` arguments to</span></span> `monitor diagnostic-settings create`

### <a name="network"></a><span data-ttu-id="a0e85-654">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-654">Network</span></span>
* <span data-ttu-id="a0e85-655">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-655">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="a0e85-656">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-656">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="a0e85-657">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a0e85-657">ServiceBus</span></span>
* <span data-ttu-id="a0e85-658">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="a0e85-658">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-659">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-659">SQL</span></span>
* <span data-ttu-id="a0e85-660">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="a0e85-660">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-661">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-661">Storage</span></span>
* <span data-ttu-id="a0e85-662">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="a0e85-662">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="a0e85-663">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="a0e85-663">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-664">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-664">VM</span></span>
* <span data-ttu-id="a0e85-665">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-665">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in</span></span> `[vm|vmss] create`
* <span data-ttu-id="a0e85-666">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-666">Updated supported size list supporting networking accelerator for</span></span> `vm create`
* <span data-ttu-id="a0e85-667">Ajout des arguments fortement typés pour les configurations E/S et Mbits/s Ultrassd pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-667">Added strong typed arguments for ultrassd iops and mbps configs for</span></span> `disk create`

## <a name="october-16-2018"></a><span data-ttu-id="a0e85-668">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-668">October 16, 2018</span></span>

<span data-ttu-id="a0e85-669">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="a0e85-669">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-670">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-670">VM</span></span>
* <span data-ttu-id="a0e85-671">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="a0e85-671">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="a0e85-672">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-672">October 9, 2018</span></span>

<span data-ttu-id="a0e85-673">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="a0e85-673">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-674">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-674">Core</span></span>
* <span data-ttu-id="a0e85-675">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="a0e85-675">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-676">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-676">ACR</span></span>
* <span data-ttu-id="a0e85-677">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="a0e85-677">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-678">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-678">ACS</span></span>
* <span data-ttu-id="a0e85-679">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="a0e85-679">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="a0e85-680">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="a0e85-680">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="a0e85-681">Modification apportée à `aks create` pour ne plus nécessiter</span><span class="sxs-lookup"><span data-stu-id="a0e85-681">Changed `aks create` to no longer require</span></span> `--aad-tenant-id`
* <span data-ttu-id="a0e85-682">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="a0e85-682">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-683">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-683">Container</span></span>
* <span data-ttu-id="a0e85-684">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="a0e85-684">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="a0e85-685">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-685">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="a0e85-686">Event Hub</span><span class="sxs-lookup"><span data-stu-id="a0e85-686">Event Hub</span></span>
* <span data-ttu-id="a0e85-687">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-687">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="a0e85-688">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="a0e85-688">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="a0e85-689">Extensions</span><span class="sxs-lookup"><span data-stu-id="a0e85-689">Extensions</span></span>
* <span data-ttu-id="a0e85-690">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="a0e85-690">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a0e85-691">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a0e85-691">HDInsight</span></span>
* <span data-ttu-id="a0e85-692">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-692">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-693">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-693">IoT</span></span>
* <span data-ttu-id="a0e85-694">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="a0e85-694">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-695">KeyVault</span></span>
* <span data-ttu-id="a0e85-696">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="a0e85-696">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-697">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-697">Network</span></span>
* <span data-ttu-id="a0e85-698">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="a0e85-698">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="a0e85-699">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="a0e85-699">See #6052</span></span>
* <span data-ttu-id="a0e85-700">Dépréciation de `--remote-vnet-id` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-700">Deprecated `--remote-vnet-id` for</span></span> `network vnet peering create`
* <span data-ttu-id="a0e85-701">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="a0e85-701">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="a0e85-702">Ajout de la prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-702">Added support for multiple subnet prefixes to `network vnet create` with</span></span> `--subnet-prefixes`
* <span data-ttu-id="a0e85-703">Ajout de la prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-703">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with</span></span> `--address-prefixes`
* <span data-ttu-id="a0e85-704">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="a0e85-704">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="a0e85-705">Ajout de l’argument d’usage `--service-endpoint-policy` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-705">Added `--service-endpoint-policy` convenience argument to</span></span> `network vnet subnet update`

### <a name="role"></a><span data-ttu-id="a0e85-706">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-706">Role</span></span>
* <span data-ttu-id="a0e85-707">Ajout de la prise en charge du listing des propriétaires d’applications Azure AD à</span><span class="sxs-lookup"><span data-stu-id="a0e85-707">Added support for listing Azure AD app owners to</span></span> `ad app owner`
* <span data-ttu-id="a0e85-708">Ajout de la prise en charge du listing des propriétaires de principaux de service Azure AD à</span><span class="sxs-lookup"><span data-stu-id="a0e85-708">Added support for listing Azure AD service principal owners to</span></span> `ad sp owner`
* <span data-ttu-id="a0e85-709">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="a0e85-709">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="a0e85-710">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="a0e85-710">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="a0e85-711">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a0e85-711">Service Bus</span></span>
* <span data-ttu-id="a0e85-712">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="a0e85-712">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-713">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-713">VM</span></span>
* <span data-ttu-id="a0e85-714">Correction du champ vide `accessSas` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-714">Fixed empty `accessSas` field in</span></span> `disk grant-access`
* <span data-ttu-id="a0e85-715">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-715">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="a0e85-716">Correction des commandes de mise à jour pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-716">Fixed update commands for</span></span> `sig`
* <span data-ttu-id="a0e85-717">Ajout de la prise en charge de `--no-wait` pour la gestion des versions d’images dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-717">Added `--no-wait` support for managing image versions in</span></span> `sig`
* <span data-ttu-id="a0e85-718">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-718">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="a0e85-719">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="a0e85-719">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="a0e85-720">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-720">September 21, 2018</span></span>

<span data-ttu-id="a0e85-721">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="a0e85-721">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-722">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-722">ACR</span></span>
* <span data-ttu-id="a0e85-723">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-723">Added ACR Task commands</span></span>
* <span data-ttu-id="a0e85-724">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="a0e85-724">Added quick run command</span></span>
* <span data-ttu-id="a0e85-725">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="a0e85-725">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="a0e85-726">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-726">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="a0e85-727">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="a0e85-727">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="a0e85-728">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="a0e85-728">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-729">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-729">ACS</span></span>
* <span data-ttu-id="a0e85-730">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-730">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="a0e85-731">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="a0e85-731">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-732">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-732">AppService</span></span>

* <span data-ttu-id="a0e85-733">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="a0e85-733">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="a0e85-734">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="a0e85-734">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="a0e85-735">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="a0e85-735">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="a0e85-736">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="a0e85-736">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-737">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-737">Batch</span></span>
* <span data-ttu-id="a0e85-738">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="a0e85-738">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="a0e85-739">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="a0e85-739">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="a0e85-740">Ajout de `--max-tasks-per-node-option` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-740">Added `--max-tasks-per-node-option` to</span></span> `batch pool create`
* <span data-ttu-id="a0e85-741">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="a0e85-741">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0e85-742">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-742">Batch AI</span></span> 
* <span data-ttu-id="a0e85-743">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-743">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0e85-744">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-744">Cognitive Services</span></span>
* <span data-ttu-id="a0e85-745">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="a0e85-745">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="a0e85-746">Ajout de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-746">Added command</span></span> `cognitiveservices account list-usage`
* <span data-ttu-id="a0e85-747">Ajout de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-747">Added command</span></span> `cognitiveservices account list-kinds`
* <span data-ttu-id="a0e85-748">Ajout de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-748">Added command</span></span> `cognitiveservices account list`
* <span data-ttu-id="a0e85-749">Déconseillé</span><span class="sxs-lookup"><span data-stu-id="a0e85-749">Deprecated</span></span> `cognitiveservices list`
* <span data-ttu-id="a0e85-750">Modification apportée à `--name` pour le rendre facultatif pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-750">Changed `--name` to be optional for</span></span> `cognitiveservices account list-skus`

### <a name="container"></a><span data-ttu-id="a0e85-751">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-751">Container</span></span>
* <span data-ttu-id="a0e85-752">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="a0e85-752">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="a0e85-753">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-753">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="a0e85-754">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a0e85-754">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="a0e85-755">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-755">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="a0e85-756">DataLake</span><span class="sxs-lookup"><span data-stu-id="a0e85-756">Datalake</span></span>
* <span data-ttu-id="a0e85-757">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a0e85-757">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="a0e85-758">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="a0e85-758">Interactive Shell</span></span>
* <span data-ttu-id="a0e85-759">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-759">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="a0e85-760">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="a0e85-760">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-761">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-761">IoT</span></span>
* <span data-ttu-id="a0e85-762">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-762">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="a0e85-763">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a0e85-763">Key Vault</span></span>
* <span data-ttu-id="a0e85-764">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="a0e85-764">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-765">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-765">Network</span></span>
* <span data-ttu-id="a0e85-766">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-766">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="a0e85-767">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="a0e85-767">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="a0e85-768">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="a0e85-768">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="a0e85-769">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-769">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="a0e85-770">Ajout de `--enable-tcp-reset` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-770">Add `--enable-tcp-reset` to</span></span> `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* <span data-ttu-id="a0e85-771">Ajout de `--disable-outbound-snat` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-771">Add `--disable-outbound-snat` to</span></span> `network lb rule create/update`
* <span data-ttu-id="a0e85-772">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-772">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="a0e85-773">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="a0e85-773">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="a0e85-774">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="a0e85-774">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* `network express-route create/update`<span data-ttu-id="a0e85-775">: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="a0e85-775">: Add `--allow-global-reach` flag</span></span>
* `network vnet subnet create/update`<span data-ttu-id="a0e85-776">: Ajout de la prise en charge pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-776">: Add support for</span></span> `--delegation`
* <span data-ttu-id="a0e85-777">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="a0e85-777">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="a0e85-778">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="a0e85-778">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="a0e85-779">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="a0e85-779">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* `dns record-set * create/update`<span data-ttu-id="a0e85-780">: Ajout de la prise en charge pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-780">: Add support for</span></span> `--target-resource`
* <span data-ttu-id="a0e85-781">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="a0e85-781">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="a0e85-782">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-782">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="a0e85-783">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="a0e85-783">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-784">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-784">RDBMS</span></span>
* <span data-ttu-id="a0e85-785">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-785">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="a0e85-786">Réservation</span><span class="sxs-lookup"><span data-stu-id="a0e85-786">Reservation</span></span>
* <span data-ttu-id="a0e85-787">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="a0e85-787">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="a0e85-788">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="a0e85-788">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="a0e85-789">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="a0e85-789">Manage App</span></span>
* <span data-ttu-id="a0e85-790">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="a0e85-790">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="a0e85-791">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="a0e85-791">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-792">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-792">Role</span></span>
* <span data-ttu-id="a0e85-793">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="a0e85-793">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="a0e85-794">SignalR</span><span class="sxs-lookup"><span data-stu-id="a0e85-794">SignalR</span></span>
* <span data-ttu-id="a0e85-795">Première version</span><span class="sxs-lookup"><span data-stu-id="a0e85-795">First release</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-796">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-796">Storage</span></span>
* <span data-ttu-id="a0e85-797">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="a0e85-797">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="a0e85-798">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="a0e85-798">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-799">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-799">VM</span></span>
* <span data-ttu-id="a0e85-800">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="a0e85-800">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="a0e85-801">Ajout de la prise en charge pour la galerie d’images partagée via</span><span class="sxs-lookup"><span data-stu-id="a0e85-801">Added support for shared image gallery through</span></span> `az sig`

## <a name="august-28-2018"></a><span data-ttu-id="a0e85-802">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-802">August 28, 2018</span></span>

<span data-ttu-id="a0e85-803">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a0e85-803">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-804">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-804">Core</span></span>

* <span data-ttu-id="a0e85-805">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="a0e85-805">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a0e85-806">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a0e85-806">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-807">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-807">ACR</span></span>

* <span data-ttu-id="a0e85-808">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="a0e85-808">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a0e85-809">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="a0e85-809">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-810">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-810">ACS</span></span>

* <span data-ttu-id="a0e85-811">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="a0e85-811">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a0e85-812">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="a0e85-812">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-813">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-813">AppService</span></span>

* <span data-ttu-id="a0e85-814">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="a0e85-814">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a0e85-815">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="a0e85-815">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a0e85-816">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-816">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a0e85-817">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a0e85-817">Backup</span></span>

* <span data-ttu-id="a0e85-818">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-818">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a0e85-819">Service de robot</span><span class="sxs-lookup"><span data-stu-id="a0e85-819">Bot Service</span></span>

* <span data-ttu-id="a0e85-820">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="a0e85-820">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0e85-821">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-821">Cognitive Services</span></span>

* <span data-ttu-id="a0e85-822">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="a0e85-822">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-823">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-823">IoT</span></span>

* <span data-ttu-id="a0e85-824">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="a0e85-824">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-825">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-825">Monitor</span></span>

* <span data-ttu-id="a0e85-826">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="a0e85-826">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a0e85-827">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="a0e85-827">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-828">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-828">Network</span></span>

* <span data-ttu-id="a0e85-829">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-829">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-830">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-830">Resource</span></span>

* <span data-ttu-id="a0e85-831">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-831">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-832">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-832">Storage</span></span>

* <span data-ttu-id="a0e85-833">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-833">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-834">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-834">VM</span></span>

* <span data-ttu-id="a0e85-835">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-835">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a0e85-836">Remplacement de `--storage-caching` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-836">Deprecated `--storage-caching` for</span></span> `vm create`

## <a name="auguest-14-2018"></a><span data-ttu-id="a0e85-837">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-837">Auguest 14, 2018</span></span>

<span data-ttu-id="a0e85-838">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a0e85-838">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-839">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-839">Core</span></span>

* <span data-ttu-id="a0e85-840">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="a0e85-840">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a0e85-841">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="a0e85-841">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a0e85-842">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="a0e85-842">Telemetry</span></span>

* <span data-ttu-id="a0e85-843">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a0e85-843">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-844">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-844">ACR</span></span>

* <span data-ttu-id="a0e85-845">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="a0e85-845">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a0e85-846">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="a0e85-846">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-847">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-847">ACS</span></span>

* <span data-ttu-id="a0e85-848">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-848">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a0e85-849">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-849">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a0e85-850">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="a0e85-850">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a0e85-851">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="a0e85-851">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a0e85-852">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="a0e85-852">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a0e85-853">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-853">AppService</span></span>

* <span data-ttu-id="a0e85-854">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="a0e85-854">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a0e85-855">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="a0e85-855">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a0e85-856">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-856">BatchAI</span></span>

* <span data-ttu-id="a0e85-857">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="a0e85-857">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a0e85-858">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-858">Container</span></span>

* <span data-ttu-id="a0e85-859">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-859">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a0e85-860">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-860">IoT</span></span>

* <span data-ttu-id="a0e85-861">[CHANGEMENT IMPORTANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="a0e85-861">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a0e85-862">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="a0e85-862">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a0e85-863">Iot Central</span><span class="sxs-lookup"><span data-stu-id="a0e85-863">Iot Central</span></span>

* <span data-ttu-id="a0e85-864">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="a0e85-864">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-865">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-865">KeyVault</span></span>


* <span data-ttu-id="a0e85-866">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="a0e85-866">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a0e85-867">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-867">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a0e85-868">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="a0e85-868">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a0e85-869">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="a0e85-869">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a0e85-870">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="a0e85-870">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a0e85-871">Relais</span><span class="sxs-lookup"><span data-stu-id="a0e85-871">Relay</span></span>

* <span data-ttu-id="a0e85-872">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-872">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-873">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-873">Sql</span></span>

* <span data-ttu-id="a0e85-874">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="a0e85-874">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-875">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-875">Storage</span></span>

* <span data-ttu-id="a0e85-876">[CHANGEMENT IMPORTANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="a0e85-876">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a0e85-877">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="a0e85-877">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a0e85-878">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="a0e85-878">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a0e85-879">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="a0e85-879">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a0e85-880">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-880">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-881">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-881">VM</span></span>

* <span data-ttu-id="a0e85-882">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="a0e85-882">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a0e85-883">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-883">July 31, 2018</span></span>

<span data-ttu-id="a0e85-884">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a0e85-884">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-885">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-885">ACR</span></span>

* <span data-ttu-id="a0e85-886">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-886">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a0e85-887">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="a0e85-887">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-888">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-888">ACS</span></span>

* <span data-ttu-id="a0e85-889">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="a0e85-889">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-890">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-890">Batch</span></span>

* <span data-ttu-id="a0e85-891">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0e85-891">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-892">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-892">Container</span></span>

* <span data-ttu-id="a0e85-893">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="a0e85-893">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-894">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-894">Network</span></span>

* <span data-ttu-id="a0e85-895">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a0e85-895">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a0e85-896">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-896">Resource</span></span>

* <span data-ttu-id="a0e85-897">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="a0e85-897">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a0e85-898">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="a0e85-898">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-899">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-899">Role</span></span>

* <span data-ttu-id="a0e85-900">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-900">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a0e85-901">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-901">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a0e85-902">Recherche</span><span class="sxs-lookup"><span data-stu-id="a0e85-902">Search</span></span>

* <span data-ttu-id="a0e85-903">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="a0e85-903">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a0e85-904">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a0e85-904">Service Bus</span></span>

* <span data-ttu-id="a0e85-905">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="a0e85-905">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a0e85-906">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-906">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  `--enable-batched-operations` <span data-ttu-id="a0e85-907">et `--enable-dead-lettering-on-message-expiration` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-907">and `--enable-dead-lettering-on-message-expiration` in</span></span> `queue`
  *  `--dead-letter-on-filter-exceptions` <span data-ttu-id="a0e85-908">commencer</span><span class="sxs-lookup"><span data-stu-id="a0e85-908">in</span></span> `subscriptions`

### <a name="storage"></a><span data-ttu-id="a0e85-909">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-909">Storage</span></span>

* <span data-ttu-id="a0e85-910">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="a0e85-910">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a0e85-911">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-911">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-912">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-912">VM</span></span>

* <span data-ttu-id="a0e85-913">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-913">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a0e85-914">Ajout de la prise en charge pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-914">Added support for</span></span> `StandardSSD_LRS`
* <span data-ttu-id="a0e85-915">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="a0e85-915">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a0e85-916">[CHANGEMENT INNOVANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-916">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a0e85-917">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-917">July 18, 2018</span></span>

<span data-ttu-id="a0e85-918">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a0e85-918">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-919">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-919">Core</span></span>

* <span data-ttu-id="a0e85-920">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-920">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a0e85-921">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a0e85-921">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a0e85-922">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="a0e85-922">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-923">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-923">ACR</span></span>

* <span data-ttu-id="a0e85-924">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="a0e85-924">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a0e85-925">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="a0e85-925">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a0e85-926">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="a0e85-926">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a0e85-927">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="a0e85-927">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-928">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-928">ACS</span></span>

* <span data-ttu-id="a0e85-929">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="a0e85-929">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-930">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-930">AppService</span></span>

* <span data-ttu-id="a0e85-931">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="a0e85-931">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-932">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-932">Batch</span></span>

* <span data-ttu-id="a0e85-933">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0e85-933">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a0e85-934">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-934">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0e85-935">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-935">Batch AI</span></span>

* <span data-ttu-id="a0e85-936">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="a0e85-936">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-937">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-937">Container</span></span>

* <span data-ttu-id="a0e85-938">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="a0e85-938">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a0e85-939">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="a0e85-939">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-940">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-940">Network</span></span>

* <span data-ttu-id="a0e85-941">Ajout de la prise en charge de `--no-wait` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-941">Added `--no-wait` support to</span></span> `network nic [create|update|delete]` 
* <span data-ttu-id="a0e85-942">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-942">Added</span></span> `network nic wait`
* <span data-ttu-id="a0e85-943">Argument `--ids` déprécié pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-943">Deprecated `--ids` argument for</span></span> `network vnet [subnet|peering] list`
* <span data-ttu-id="a0e85-944">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de</span><span class="sxs-lookup"><span data-stu-id="a0e85-944">Added `--include-default` flag to include default security rules in the output of</span></span> `network nsg rule list`  

### <a name="resource"></a><span data-ttu-id="a0e85-945">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-945">Resource</span></span>

* <span data-ttu-id="a0e85-946">Ajout de la prise en charge de `--no-wait` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-946">Added `--no-wait` support to</span></span> `group deployment delete`
* <span data-ttu-id="a0e85-947">Ajout de la prise en charge de `--no-wait` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-947">Added `--no-wait` support to</span></span> `deployment delete`
* <span data-ttu-id="a0e85-948">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="a0e85-948">Added `deployment wait` command</span></span>
* <span data-ttu-id="a0e85-949">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="a0e85-949">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-950">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-950">SQL</span></span>

* <span data-ttu-id="a0e85-951">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-951">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a0e85-952">Autoriser la configuration de SQL Server par défaut en exécutant</span><span class="sxs-lookup"><span data-stu-id="a0e85-952">Allow configuring default sql server by executing</span></span> `az configure --defaults sql-server=<name>`
* <span data-ttu-id="a0e85-953">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="a0e85-953">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-954">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-954">Storage</span></span>

* <span data-ttu-id="a0e85-955">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="a0e85-955">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-956">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-956">VM</span></span>

* <span data-ttu-id="a0e85-957">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-957">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a0e85-958">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-958">Added `--no-wait` support to `vm extension [set|delete]` and</span></span> `vmss extension [set|delete]`
* <span data-ttu-id="a0e85-959">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-959">Added</span></span> `vm extension wait`

## <a name="july-3-2018"></a><span data-ttu-id="a0e85-960">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-960">July 3, 2018</span></span>

<span data-ttu-id="a0e85-961">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a0e85-961">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a0e85-962">AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-962">AKS</span></span>

* <span data-ttu-id="a0e85-963">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-963">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a0e85-964">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-964">July 3, 2018</span></span>

<span data-ttu-id="a0e85-965">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a0e85-965">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-966">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-966">Core</span></span>

* <span data-ttu-id="a0e85-967">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-967">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-968">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-968">ACR</span></span>

* <span data-ttu-id="a0e85-969">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="a0e85-969">Added polling build status</span></span>
* <span data-ttu-id="a0e85-970">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-970">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a0e85-971">Ajout des paramètres `--top` et `--orderby` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-971">Added `--top` and `--orderby` parameters for</span></span> `show-manifests`

### <a name="acs"></a><span data-ttu-id="a0e85-972">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-972">ACS</span></span>

* <span data-ttu-id="a0e85-973">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-973">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a0e85-974">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-974">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a0e85-975">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-975">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a0e85-976">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="a0e85-976">Added `--listen-port` support</span></span>
* <span data-ttu-id="a0e85-977">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-977">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a0e85-978">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="a0e85-978">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a0e85-979">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="a0e85-979">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-980">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-980">AppService</span></span>

* <span data-ttu-id="a0e85-981">Ajout de la prise en charge de la désactivation de la fonctionnalité Identity via</span><span class="sxs-lookup"><span data-stu-id="a0e85-981">Added support for disabling identity via</span></span> `webapp identity remove`
* <span data-ttu-id="a0e85-982">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="a0e85-982">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a0e85-983">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a0e85-983">Backup</span></span>

* <span data-ttu-id="a0e85-984">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="a0e85-984">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a0e85-985">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-985">BatchAI</span></span>

* <span data-ttu-id="a0e85-986">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="a0e85-986">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a0e85-987">Cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-987">Cloud</span></span>

* <span data-ttu-id="a0e85-988">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-988">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-989">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-989">Container</span></span>

* <span data-ttu-id="a0e85-990">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="a0e85-990">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a0e85-991">Ajout des paramètres Log Analytics `--log-analytics-workspace` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-991">Added Log Analytics parameters `--log-analytics-workspace` and</span></span> `--log-analytics-workspace-key`
* <span data-ttu-id="a0e85-992">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="a0e85-992">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-993">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-993">Extension</span></span>

* <span data-ttu-id="a0e85-994">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="a0e85-994">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-995">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-995">Network</span></span>

* <span data-ttu-id="a0e85-996">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="a0e85-996">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-997">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a0e85-997">Rdbms</span></span>

* <span data-ttu-id="a0e85-998">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a0e85-998">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-999">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-999">Resource</span></span>

* <span data-ttu-id="a0e85-1000">Ajout d’un nouveau groupe d’opérations</span><span class="sxs-lookup"><span data-stu-id="a0e85-1000">Added new operation group</span></span> `deployment`

### <a name="vm"></a><span data-ttu-id="a0e85-1001">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1001">VM</span></span>

* <span data-ttu-id="a0e85-1002">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="a0e85-1002">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a0e85-1003">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1003">June 25, 2018</span></span>

<span data-ttu-id="a0e85-1004">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a0e85-1004">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a0e85-1005">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1005">CLI</span></span>

* <span data-ttu-id="a0e85-1006">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1006">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a0e85-1007">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1007">June 19, 2018</span></span>

<span data-ttu-id="a0e85-1008">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a0e85-1008">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1009">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1009">Core</span></span>

* <span data-ttu-id="a0e85-1010">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1010">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1011">ACR</span></span>

* <span data-ttu-id="a0e85-1012">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="a0e85-1012">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a0e85-1013">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1013">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1014">ACS</span></span>

* <span data-ttu-id="a0e85-1015">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1015">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a0e85-1016">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1016">Added `--update` support</span></span>
* <span data-ttu-id="a0e85-1017">Modification apportée à `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1017">Changed `aks get-credentials --admin` to not eplace the user context in</span></span> `$HOME/.kube/config`
* <span data-ttu-id="a0e85-1018">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1018">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a0e85-1019">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1019">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a0e85-1020">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1020">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and</span></span> `aks remove-connector`
* <span data-ttu-id="a0e85-1021">Ajout de nouvelles régions Azure Container Instance pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1021">Added new Azure Container Instance regions for</span></span> `aks install-connector`
* <span data-ttu-id="a0e85-1022">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1022">Added the normalized location into the helm release name and node name to</span></span> `aks install-connector`

### <a name="appservice"></a><span data-ttu-id="a0e85-1023">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1023">AppService</span></span>

* <span data-ttu-id="a0e85-1024">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1024">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a0e85-1025">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1025">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-1026">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1026">Batch</span></span>

* <span data-ttu-id="a0e85-1027">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1027">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0e85-1028">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1028">Batch AI</span></span>

* <span data-ttu-id="a0e85-1029">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1029">Added support for workspaces.</span></span> <span data-ttu-id="a0e85-1030">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1030">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a0e85-1031">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1031">Added support for experiments.</span></span> <span data-ttu-id="a0e85-1032">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1032">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a0e85-1033">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="a0e85-1033">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a0e85-1034">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1034">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a0e85-1035">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1035">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a0e85-1036">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1036">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a0e85-1037">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1037">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a0e85-1038">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="a0e85-1038">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a0e85-1039">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1039">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a0e85-1040">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1040">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a0e85-1041">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1041">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a0e85-1042">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1042">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a0e85-1043">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1043">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a0e85-1044">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1044">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a0e85-1045">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1045">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a0e85-1046">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1046">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="a0e85-1047">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1047">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="a0e85-1048">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1048">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a0e85-1049">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1049">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a0e85-1050">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1050">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a0e85-1051">Cartes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1051">Maps</span></span>

* <span data-ttu-id="a0e85-1052">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1052">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1053">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1053">Network</span></span>

* <span data-ttu-id="a0e85-1054">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1054">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a0e85-1055">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1055">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a0e85-1056">#6502</span><span class="sxs-lookup"><span data-stu-id="a0e85-1056">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a0e85-1057">Réservations</span><span class="sxs-lookup"><span data-stu-id="a0e85-1057">Reservations</span></span>

* <span data-ttu-id="a0e85-1058">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1058">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to</span></span> `reservations catalog show`
* <span data-ttu-id="a0e85-1059">Ajout du paramètre `Location` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1059">Added parameter `Location`to</span></span> `reservations catalog show`
* <span data-ttu-id="a0e85-1060">[CHANGEMENT CASSANT] Suppression de `kind` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1060">[BREAKING CHANGE] Removed `kind` from</span></span> `ReservationProperties`
* <span data-ttu-id="a0e85-1061">[CHANGEMENT CASSANT] Renommage de `capabilities` en `sku_properties` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1061">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in</span></span> `Catalog`
* <span data-ttu-id="a0e85-1062">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1062">[BREAKING CHANGE] Removed `size` and `tier` properties from</span></span> `Catalog`
* <span data-ttu-id="a0e85-1063">Ajout du paramètre `InstanceFlexibility` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1063">Added parameter `InstanceFlexibility` to</span></span> `reservations reservation update`

### <a name="role"></a><span data-ttu-id="a0e85-1064">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1064">Role</span></span>

* <span data-ttu-id="a0e85-1065">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1065">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1066">SQL</span></span>

* <span data-ttu-id="a0e85-1067">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1067">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1068">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1068">Storage</span></span>

* <span data-ttu-id="a0e85-1069">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="a0e85-1069">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1070">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1070">VM</span></span>

* <span data-ttu-id="a0e85-1071">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1071">Improved refine vm size check for accelerated networking support in</span></span> `vm create`
* <span data-ttu-id="a0e85-1072">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1072">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to</span></span> `Standard_DS1_v2`
* <span data-ttu-id="a0e85-1073">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1073">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a0e85-1074">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1074">June 13, 2018</span></span>

<span data-ttu-id="a0e85-1075">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a0e85-1075">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1076">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1076">Core</span></span>

* <span data-ttu-id="a0e85-1077">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1077">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a0e85-1078">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1078">June 13, 2018</span></span>

<span data-ttu-id="a0e85-1079">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a0e85-1079">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a0e85-1080">AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1080">AKS</span></span>

* <span data-ttu-id="a0e85-1081">Ajout d’options réseau avancées à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1081">Added advanced networking options to</span></span> `aks create`
* <span data-ttu-id="a0e85-1082">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="a0e85-1082">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a0e85-1083">Ajout de l’argument `--no-ssh-key` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1083">Added `--no-ssh-key` argument to</span></span> `aks create`
* <span data-ttu-id="a0e85-1084">Ajout de l’argument `--enable-rbac` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1084">Added `--enable-rbac` argument to</span></span> `aks create`
* <span data-ttu-id="a0e85-1085">[PRÉVERSION] Ajout de la prise en charge de l’authentification basée sur Azure Active Directory à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1085">[PREVIEW] Added support for Azure Active Directory authentication to</span></span> `aks create`

### <a name="appservice"></a><span data-ttu-id="a0e85-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1086">AppService</span></span>

* <span data-ttu-id="a0e85-1087">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="a0e85-1087">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a0e85-1088">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1088">June 5, 2018</span></span>

<span data-ttu-id="a0e85-1089">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a0e85-1089">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1090">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1090">Interactive</span></span>

* <span data-ttu-id="a0e85-1091">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a0e85-1091">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a0e85-1092">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1092">June 5, 2018</span></span>

<span data-ttu-id="a0e85-1093">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a0e85-1093">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1094">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1094">Core</span></span>

* <span data-ttu-id="a0e85-1095">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="a0e85-1095">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a0e85-1096">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a0e85-1096">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1097">ACR</span></span>

* <span data-ttu-id="a0e85-1098">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="a0e85-1098">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a0e85-1099">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1099">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a0e85-1100">AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1100">AKS</span></span>

* <span data-ttu-id="a0e85-1101">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1101">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-1102">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1102">Batch</span></span>

* <span data-ttu-id="a0e85-1103">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1103">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-1104">IOT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1104">IOT</span></span>

* <span data-ttu-id="a0e85-1105">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="a0e85-1105">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1106">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1106">Network</span></span>

* <span data-ttu-id="a0e85-1107">Amélioré</span><span class="sxs-lookup"><span data-stu-id="a0e85-1107">Improved</span></span> `network vnet peering`

### <a name="policy-insights"></a><span data-ttu-id="a0e85-1108">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a0e85-1108">Policy Insights</span></span>

* <span data-ttu-id="a0e85-1109">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1109">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a0e85-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="a0e85-1110">ARM</span></span>

* <span data-ttu-id="a0e85-1111">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1111">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1112">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1112">SQL</span></span>

* <span data-ttu-id="a0e85-1113">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1113">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a0e85-1114">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1114">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a0e85-1115">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1115">Storage</span></span>

* <span data-ttu-id="a0e85-1116">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="a0e85-1116">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1117">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1117">VM</span></span>

* <span data-ttu-id="a0e85-1118">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1118">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a0e85-1119">Ajout de l’option `--accelerated-networking` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1119">Added `--accelerated-networking` option to</span></span> `vm create`
* <span data-ttu-id="a0e85-1120">Ajout de `--tags` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1120">Added `--tags` to</span></span> `identity create`

## <a name="may-22-2018"></a><span data-ttu-id="a0e85-1121">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1121">May 22, 2018</span></span>

<span data-ttu-id="a0e85-1122">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a0e85-1122">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1123">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1123">Core</span></span>

* <span data-ttu-id="a0e85-1124">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="a0e85-1124">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1125">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1125">ACS</span></span>

* <span data-ttu-id="a0e85-1126">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1126">Added new Dev-Spaces commands `aks use-dev-spaces` and</span></span> `aks remove-dev-spaces`
* <span data-ttu-id="a0e85-1127">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="a0e85-1127">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1128">AppService</span></span>

* <span data-ttu-id="a0e85-1129">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="a0e85-1129">Improved generic update commands</span></span>
* <span data-ttu-id="a0e85-1130">Ajout de la prise en charge asynchrone pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1130">Added async support for</span></span> `webapp deployment source config-zip`

### <a name="container"></a><span data-ttu-id="a0e85-1131">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1131">Container</span></span>

* <span data-ttu-id="a0e85-1132">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="a0e85-1132">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a0e85-1133">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1133">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1134">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1134">Extension</span></span>

* <span data-ttu-id="a0e85-1135">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="a0e85-1135">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1136">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1136">Interactive</span></span>

* <span data-ttu-id="a0e85-1137">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-1137">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a0e85-1138">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="a0e85-1138">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-1139">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-1139">KeyVault</span></span>

* <span data-ttu-id="a0e85-1140">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a0e85-1140">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1141">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1141">Network</span></span>

* <span data-ttu-id="a0e85-1142">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1142">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a0e85-1143">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1143">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1144">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1144">SQL</span></span>

* <span data-ttu-id="a0e85-1145">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1145">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a0e85-1146">Propriété `serviceLevelObjective` renommée en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1146">Renamed `serviceLevelObjective` property to</span></span> `currentServiceObjectiveName`
    * <span data-ttu-id="a0e85-1147">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1147">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a0e85-1148">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a0e85-1148">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a0e85-1149">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1149">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * `requestedServiceObjectiveName`<span data-ttu-id="a0e85-1150">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1150">.</span></span>  <span data-ttu-id="a0e85-1151">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1151">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * `edition`<span data-ttu-id="a0e85-1152">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1152">.</span></span> <span data-ttu-id="a0e85-1153">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1153">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * `elasticPoolName`<span data-ttu-id="a0e85-1154">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1154">.</span></span> <span data-ttu-id="a0e85-1155">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1155">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a0e85-1156">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1156">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * `edition`<span data-ttu-id="a0e85-1157">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1157">.</span></span> <span data-ttu-id="a0e85-1158">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1158">To update, use the `--edition` parameter</span></span>
    * `dtu`<span data-ttu-id="a0e85-1159">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1159">.</span></span> <span data-ttu-id="a0e85-1160">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1160">To update, use the `--capacity` parameter</span></span>
    *  `databaseDtuMin`<span data-ttu-id="a0e85-1161">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1161">.</span></span> <span data-ttu-id="a0e85-1162">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1162">To update, use the `--db-min-capacity` parameter</span></span>
    *  `databaseDtuMax`<span data-ttu-id="a0e85-1163">.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1163">.</span></span> <span data-ttu-id="a0e85-1164">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1164">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a0e85-1165">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1165">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a0e85-1166">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1166">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1167">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1167">Storage</span></span>

* <span data-ttu-id="a0e85-1168">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1168">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a0e85-1169">Correction d’un problème avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1169">Fixed problem with</span></span> `storage entity query`

### <a name="vm"></a><span data-ttu-id="a0e85-1170">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1170">VM</span></span>

* <span data-ttu-id="a0e85-1171">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1171">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a0e85-1172">La même prise en charge est accessible via `vm update` ou</span><span class="sxs-lookup"><span data-stu-id="a0e85-1172">The same support can be accessed through `vm update` or</span></span> `vm disk attach`
* <span data-ttu-id="a0e85-1173">Mise en correspondance de l’image de l’extension dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1173">Fixed extension image matching in</span></span> `[vm|vmss] extension`
* <span data-ttu-id="a0e85-1174">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1174">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a0e85-1175">Ajout de `--license-type` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1175">Added `--license-type` to</span></span> `[vm|vmss] update`

## <a name="may-7-2018"></a><span data-ttu-id="a0e85-1176">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1176">May 7, 2018</span></span>

<span data-ttu-id="a0e85-1177">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a0e85-1177">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1178">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1178">Core</span></span>

* <span data-ttu-id="a0e85-1179">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="a0e85-1179">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a0e85-1180">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="a0e85-1180">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a0e85-1181">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1181">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a0e85-1182">#5591</span><span class="sxs-lookup"><span data-stu-id="a0e85-1182">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a0e85-1183">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1183">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a0e85-1184">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="a0e85-1184">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a0e85-1185">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1185">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a0e85-1186">Amélioration de l’erreur lorsque les utilisateurs entrent</span><span class="sxs-lookup"><span data-stu-id="a0e85-1186">Improved error when users type</span></span> `az ''`
* <span data-ttu-id="a0e85-1187">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1187">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1188">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1188">ACR</span></span>

* <span data-ttu-id="a0e85-1189">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1189">Added ACR Build commands</span></span>
* <span data-ttu-id="a0e85-1190">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="a0e85-1190">Improved resource not found error messages</span></span>
* <span data-ttu-id="a0e85-1191">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1191">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a0e85-1192">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1192">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a0e85-1193">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="a0e85-1193">Improved repository commands error messages</span></span>
* <span data-ttu-id="a0e85-1194">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1194">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1195">ACS</span></span>

* <span data-ttu-id="a0e85-1196">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="a0e85-1196">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a0e85-1197">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="a0e85-1197">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a0e85-1198">AMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1198">AMS</span></span>

* <span data-ttu-id="a0e85-1199">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-1199">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1200">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1200">Appservice</span></span>

* <span data-ttu-id="a0e85-1201">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="a0e85-1201">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a0e85-1202">Suppression de `--runtime-version` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1202">Removed `--runtime-version` from</span></span> `webapp auth update`
* <span data-ttu-id="a0e85-1203">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="a0e85-1203">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a0e85-1204">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1204">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a0e85-1205">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1205">Batch AI</span></span>

* <span data-ttu-id="a0e85-1206">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="a0e85-1206">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0e85-1207">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-1207">Cognitive Services</span></span>

* <span data-ttu-id="a0e85-1208">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1208">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a0e85-1209">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1209">Consumption</span></span>

* <span data-ttu-id="a0e85-1210">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="a0e85-1210">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1211">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1211">Container</span></span>

* <span data-ttu-id="a0e85-1212">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="a0e85-1212">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a0e85-1213">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0e85-1213">Cosmos DB</span></span>

* <span data-ttu-id="a0e85-1214">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a0e85-1214">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a0e85-1215">DMS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1215">DMS</span></span>

* <span data-ttu-id="a0e85-1216">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="a0e85-1216">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1217">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1217">Extension</span></span>

* <span data-ttu-id="a0e85-1218">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1218">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1219">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1219">Interactive</span></span>

* <span data-ttu-id="a0e85-1220">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="a0e85-1220">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a0e85-1221">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="a0e85-1221">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a0e85-1222">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="a0e85-1222">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a0e85-1223">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1223">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a0e85-1224">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-1224">Lab</span></span>

* <span data-ttu-id="a0e85-1225">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="a0e85-1225">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1226">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1226">Network</span></span>

* <span data-ttu-id="a0e85-1227">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1227">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a0e85-1228">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1228">Profile</span></span>

* <span data-ttu-id="a0e85-1229">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1229">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a0e85-1230">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1230">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a0e85-1231">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1231">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a0e85-1232">Redis</span><span class="sxs-lookup"><span data-stu-id="a0e85-1232">Redis</span></span>

* <span data-ttu-id="a0e85-1233">Dépréciation de `redis patch-schedule patch-schedule show` en faveur de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1233">Deprecated `redis patch-schedule patch-schedule show` in favor of</span></span> `redis patch-schedule show`
* <span data-ttu-id="a0e85-1234">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1234">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a0e85-1235">Cette fonctionnalité a été placée dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1235">This functionality has been folded into</span></span> `redis list`
* <span data-ttu-id="a0e85-1236">Dépréciation de `redis import-method` en faveur de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1236">Deprecated `redis import-method` in favor of</span></span> `redis import`
* <span data-ttu-id="a0e85-1237">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1237">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-1238">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1238">Role</span></span>

* <span data-ttu-id="a0e85-1239">[CHANGEMENT CASSANT] Suppression due à la dépréciation de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1239">[BREAKING CHANGE] Removed deprecated</span></span> `ad sp reset-credentials`

### <a name="storage"></a><span data-ttu-id="a0e85-1240">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1240">Storage</span></span>

* <span data-ttu-id="a0e85-1241">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1241">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a0e85-1242">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="a0e85-1242">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a0e85-1243">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1243">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a0e85-1244">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="a0e85-1244">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a0e85-1245">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1245">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1246">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1246">VM</span></span>

* <span data-ttu-id="a0e85-1247">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1247">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a0e85-1248">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1248">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a0e85-1249">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1249">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a0e85-1250">Ajout de la prise en charge de la stratégie d’éviction dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1250">Added support for eviction policy to</span></span> `vmss`
* <span data-ttu-id="a0e85-1251">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1251">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a0e85-1252">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="a0e85-1252">Added write accelerator support</span></span>
* <span data-ttu-id="a0e85-1253">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-1253">Added</span></span> `vmss perform-maintenance`
* <span data-ttu-id="a0e85-1254">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1254">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a0e85-1255">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="a0e85-1255">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a0e85-1256">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1256">April 10, 2018</span></span>

<span data-ttu-id="a0e85-1257">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a0e85-1257">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1258">ACR</span></span>

* <span data-ttu-id="a0e85-1259">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="a0e85-1259">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1260">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1260">ACS</span></span>

* <span data-ttu-id="a0e85-1261">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1261">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1262">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1262">Appservice</span></span>

* [<span data-ttu-id="a0e85-1263">CHANGEMENT CASSANT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1263">BREAKING CHANGE</span></span>]: Removed `assign-identity`
* <span data-ttu-id="a0e85-1264">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="a0e85-1264">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a0e85-1265">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1265">BatchAI</span></span>

* <span data-ttu-id="a0e85-1266">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="a0e85-1266">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="a0e85-1267">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1267">Job level mounting</span></span>
  - <span data-ttu-id="a0e85-1268">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="a0e85-1268">Environment variables with secret values</span></span>
  - <span data-ttu-id="a0e85-1269">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="a0e85-1269">Performance counters settings</span></span>
  - <span data-ttu-id="a0e85-1270">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1270">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="a0e85-1271">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="a0e85-1271">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="a0e85-1272">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="a0e85-1272">Usage and limits reporting</span></span>
  - <span data-ttu-id="a0e85-1273">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1273">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="a0e85-1274">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1274">Support for custom images</span></span>
  - <span data-ttu-id="a0e85-1275">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1275">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a0e85-1276">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1276">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a0e85-1277">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="a0e85-1277">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a0e85-1278">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="a0e85-1278">National clouds are supported</span></span>
* <span data-ttu-id="a0e85-1279">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="a0e85-1279">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a0e85-1280">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1280">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a0e85-1281">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1281">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a0e85-1282">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1282">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a0e85-1283">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1283">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a0e85-1284">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1284">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a0e85-1285">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1285">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a0e85-1286">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1286">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a0e85-1287">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="a0e85-1287">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a0e85-1288">Ajout de l’option `--generate-ssh-keys` à `cluster create` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1288">Added `--generate-ssh-keys` option to `cluster create` and</span></span> `file-server create`
* <span data-ttu-id="a0e85-1289">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1289">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a0e85-1290">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1290">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a0e85-1291">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1291">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a0e85-1292">Facturation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1292">Billing</span></span>

* <span data-ttu-id="a0e85-1293">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="a0e85-1293">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a0e85-1294">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1294">Consumption</span></span>

* <span data-ttu-id="a0e85-1295">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1295">Added `marketplace` commands</span></span>
* <span data-ttu-id="a0e85-1296">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1296">[BREAKING CHANGE] Renamed `reservations summaries` to</span></span> `reservation summary`
* <span data-ttu-id="a0e85-1297">[CHANGEMENT CASSANT] Renommage de `reservations details` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1297">[BREAKING CHANGE] Renamed `reservations details` to</span></span> `reservation detail`
* <span data-ttu-id="a0e85-1298">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1298">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a0e85-1299">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1299">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a0e85-1300">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1300">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1301">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1301">Container</span></span>

* <span data-ttu-id="a0e85-1302">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1302">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and</span></span> `--gitrepo-mount-path`
* <span data-ttu-id="a0e85-1303">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="a0e85-1303">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1304">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1304">Extension</span></span>

* <span data-ttu-id="a0e85-1305">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1305">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1306">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1306">Interactive</span></span>

* <span data-ttu-id="a0e85-1307">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="a0e85-1307">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a0e85-1308">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1308">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a0e85-1309">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1309">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1310">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1310">Network</span></span>

* <span data-ttu-id="a0e85-1311">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="a0e85-1311">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a0e85-1312">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1312">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a0e85-1313">#4910</span><span class="sxs-lookup"><span data-stu-id="a0e85-1313">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a0e85-1314">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1314">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a0e85-1315">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1315">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a0e85-1316">Résolution du problème avec l’indicateur `--disable-bgp-route-propagation` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1316">Fixed issue with `--disable-bgp-route-propagation` flag in</span></span> `network route-table [create|update]`
* <span data-ttu-id="a0e85-1317">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1317">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for</span></span> `network lb [create|update]`
* <span data-ttu-id="a0e85-1318">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 dans `network dns zone [import|export]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1318">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and</span></span> `network dns record-set txt add-record`

### <a name="profile"></a><span data-ttu-id="a0e85-1319">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1319">Profile</span></span>

* <span data-ttu-id="a0e85-1320">Ajout de la prise en charge des comptes Azure Classic dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1320">Added support for Azure Classic accounts in</span></span> `account list`
* <span data-ttu-id="a0e85-1321">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1321">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-1322">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1322">RDBMS</span></span>

* <span data-ttu-id="a0e85-1323">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1323">Added `georestore` command</span></span>
* <span data-ttu-id="a0e85-1324">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1324">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1325">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1325">Resource</span></span>

* <span data-ttu-id="a0e85-1326">Ajout de la prise en charge de `--metadata` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1326">Added support for `--metadata` to</span></span> `policy definition create`
* <span data-ttu-id="a0e85-1327">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1327">Added support for `--metadata`, `--set`, `--add`, `--remove` to</span></span> `policy definition update`

### <a name="sql"></a><span data-ttu-id="a0e85-1328">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1328">SQL</span></span>

* <span data-ttu-id="a0e85-1329">Ajout de `sql elastic-pool op list` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1329">Added `sql elastic-pool op list` and</span></span> `sql elastic-pool op cancel`

### <a name="storage"></a><span data-ttu-id="a0e85-1330">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1330">Storage</span></span>

* <span data-ttu-id="a0e85-1331">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1331">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1332">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1332">VM</span></span>

* <span data-ttu-id="a0e85-1333">Ajout de la prise en charge de la configuration du nombre de domaines d’erreur de plateforme sur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1333">Added support to configure platform fault domain count to</span></span> `vmss create`
* <span data-ttu-id="a0e85-1334">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1334">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [<span data-ttu-id="a0e85-1335">CHANGEMENT CASSANT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1335">BREAKING CHANGE</span></span>]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="a0e85-1336">Ajout de la prise en charge des références SKU d’IP public à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1336">Added support for Public-IP SKU to</span></span> `vm create`
* <span data-ttu-id="a0e85-1337">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1337">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a0e85-1338">#5718</span><span class="sxs-lookup"><span data-stu-id="a0e85-1338">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a0e85-1339">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="a0e85-1339">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a0e85-1340">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1340">March 27, 2018</span></span>

<span data-ttu-id="a0e85-1341">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a0e85-1341">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1342">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1342">Core</span></span>

* <span data-ttu-id="a0e85-1343">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="a0e85-1343">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1344">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1344">ACS</span></span>

* <span data-ttu-id="a0e85-1345">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0e85-1345">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1346">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1346">Appservice</span></span>

* <span data-ttu-id="a0e85-1347">Ajout de la prise en charge HTTPS exclusive à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1347">Added HTTPS-only support to</span></span> `webapp update`
* <span data-ttu-id="a0e85-1348">Ajout de la prise en charge des emplacements dans `az webapp identity [assign|show]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1348">Added support for slots to `az webapp identity [assign|show]` and</span></span> `az functionapp identity [assign|show]`

### <a name="backup"></a><span data-ttu-id="a0e85-1349">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a0e85-1349">Backup</span></span>

* <span data-ttu-id="a0e85-1350">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1350">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a0e85-1351">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1351">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a0e85-1352">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1352">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a0e85-1353">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1353">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1354">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1354">Container</span></span>

* <span data-ttu-id="a0e85-1355">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1355">Added `container exec` command.</span></span> <span data-ttu-id="a0e85-1356">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1356">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a0e85-1357">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1357">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1358">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1358">Extension</span></span>

* <span data-ttu-id="a0e85-1359">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="a0e85-1359">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a0e85-1360">Modification apportée à `extension list-available` afin d’afficher les données complètes d’extension avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1360">Changed `extension list-available` to show full extension data with</span></span> `--show-details`
* <span data-ttu-id="a0e85-1361">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1361">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1362">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1362">Interactive</span></span>

* <span data-ttu-id="a0e85-1363">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1363">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a0e85-1364">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1364">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a0e85-1365">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="a0e85-1365">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a0e85-1366">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="a0e85-1366">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a0e85-1367">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-1367">Lab</span></span>

* <span data-ttu-id="a0e85-1368">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1368">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1369">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1369">Monitor</span></span>

* <span data-ttu-id="a0e85-1370">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1370">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a0e85-1371">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="a0e85-1371">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a0e85-1372">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1372">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1373">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1373">Network</span></span>

* <span data-ttu-id="a0e85-1374">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1374">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a0e85-1375">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1375">Profile</span></span>

* <span data-ttu-id="a0e85-1376">Ajout d’un avertissement pour `--identity-port` et `--msi-port` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1376">Added warning for `--identity-port` and `--msi-port` to</span></span> `login`

### <a name="rdbms"></a><span data-ttu-id="a0e85-1377">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1377">RDBMS</span></span>

* <span data-ttu-id="a0e85-1378">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a0e85-1378">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1379">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1379">Resource</span></span>

* [<span data-ttu-id="a0e85-1380">CHANGEMENT CASSANT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1380">BREAKING CHANGE</span></span>]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a0e85-1381">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1381">Role</span></span>

* <span data-ttu-id="a0e85-1382">Ajout de la prise en charge des configurations d’accès et des clients natifs requis dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1382">Added support for required access configurations and native clients to</span></span> `az ad app create`
* <span data-ttu-id="a0e85-1383">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="a0e85-1383">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a0e85-1384">Ajout des commandes de gestion des informations d’identification</span><span class="sxs-lookup"><span data-stu-id="a0e85-1384">Added credential management commands</span></span> `ad sp credential [reset|list|delete]`
* <span data-ttu-id="a0e85-1385">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1385">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a0e85-1386">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1386">Added support for `dataActions` and `notDataActions` permissions to</span></span> `role definition`

### <a name="storage"></a><span data-ttu-id="a0e85-1387">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1387">Storage</span></span>

* <span data-ttu-id="a0e85-1388">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="a0e85-1388">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a0e85-1389">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="a0e85-1389">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1390">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1390">VM</span></span>

* <span data-ttu-id="a0e85-1391">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="a0e85-1391">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a0e85-1392">Ajout de la prise en charge de la résilience dans la zone à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1392">Added zone resilient support to</span></span> `vm [snapshot|image]`
* <span data-ttu-id="a0e85-1393">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1393">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a0e85-1394">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="a0e85-1394">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a0e85-1395">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1395">March 13, 2018</span></span>

<span data-ttu-id="a0e85-1396">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a0e85-1396">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1397">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1397">ACR</span></span>

* <span data-ttu-id="a0e85-1398">Ajout de la prise en charge du paramètre `--image` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1398">Added support for `--image` parameter to</span></span> `repository delete`
* <span data-ttu-id="a0e85-1399">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1399">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a0e85-1400">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="a0e85-1400">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1401">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1401">ACS</span></span>

* <span data-ttu-id="a0e85-1402">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="a0e85-1402">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a0e85-1403">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="a0e85-1403">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a0e85-1404">Advisor</span><span class="sxs-lookup"><span data-stu-id="a0e85-1404">Advisor</span></span>

* <span data-ttu-id="a0e85-1405">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1405">[BREAKING CHANGE] Renamed `advisor configuration get` to</span></span> `advisor configuration list`
* <span data-ttu-id="a0e85-1406">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1406">[BREAKING CHANGE] Renamed `advisor configuration set` to</span></span> `advisor configuration update`
* <span data-ttu-id="a0e85-1407">[CHANGEMENT CASSANT] Suppression de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1407">[BREAKING CHANGE] Removed</span></span> `advisor recommendation generate`
* <span data-ttu-id="a0e85-1408">Ajout du paramètre `--refresh` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1408">Added `--refresh` parameter to</span></span> `advisor recommendation list`
* <span data-ttu-id="a0e85-1409">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1409">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1410">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1410">Appservice</span></span>

* <span data-ttu-id="a0e85-1411">Déconseillé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1411">Deprecated</span></span> `[webapp|functionapp] assign-identity`
* <span data-ttu-id="a0e85-1412">Ajout des commandes Managed Identity `webapp identity [assign|show]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1412">Added managed identity commands `webapp identity [assign|show]` and</span></span> `functionapp identity [assign|show]`

### <a name="eventhubs"></a><span data-ttu-id="a0e85-1413">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1413">Eventhubs</span></span>

* <span data-ttu-id="a0e85-1414">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1414">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1415">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1415">Extension</span></span>

* <span data-ttu-id="a0e85-1416">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1416">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1417">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1417">Interactive</span></span>

* <span data-ttu-id="a0e85-1418">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="a0e85-1418">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a0e85-1419">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1419">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a0e85-1420">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="a0e85-1420">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a0e85-1421">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="a0e85-1421">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1422">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1422">Monitor</span></span>

* <span data-ttu-id="a0e85-1423">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1423">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a0e85-1424">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1424">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a0e85-1425">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1425">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a0e85-1426">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1426">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1427">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1427">Network</span></span>

* <span data-ttu-id="a0e85-1428">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1428">[BREAKING CHANGE] Removed `--tags` parameter from</span></span>  `route-filter rule create`
* <span data-ttu-id="a0e85-1429">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1429">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a0e85-1430">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1430">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a0e85-1431">Ajout des paramètres `--vnet` et `--subnet` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1431">Added `--vnet` and `--subnet` parameters to</span></span> `network watcher show-topology`

### <a name="profile"></a><span data-ttu-id="a0e85-1432">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1432">Profile</span></span>

* <span data-ttu-id="a0e85-1433">Paramètre `--msi` déprécié pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1433">Deprecated `--msi` parameter for</span></span> `az login`
* <span data-ttu-id="a0e85-1434">Ajout du paramètre `--identity` pour `az login` afin de remplacer</span><span class="sxs-lookup"><span data-stu-id="a0e85-1434">Added `--identity` parameter for `az login` to replace</span></span> `--msi`

### <a name="rdbms"></a><span data-ttu-id="a0e85-1435">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1435">RDBMS</span></span>

* <span data-ttu-id="a0e85-1436">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="a0e85-1436">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a0e85-1437">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a0e85-1437">Service Bus</span></span>

* <span data-ttu-id="a0e85-1438">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1438">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1439">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1439">Storage</span></span>

* <span data-ttu-id="a0e85-1440">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="a0e85-1440">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a0e85-1441">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="a0e85-1441">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1442">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1442">VM</span></span>

* <span data-ttu-id="a0e85-1443">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="a0e85-1443">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a0e85-1444">Dépréciation de `[vm|vmss] assign-identity` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1444">Deprecated `[vm|vmss] assign-identity` and</span></span> `[vm|vmss] remove-identity`
* <span data-ttu-id="a0e85-1445">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1445">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a0e85-1446">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="a0e85-1446">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a0e85-1447">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1447">February 27, 2018</span></span>

<span data-ttu-id="a0e85-1448">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a0e85-1448">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1449">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1449">Core</span></span>

* <span data-ttu-id="a0e85-1450">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="a0e85-1450">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a0e85-1451">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1451">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a0e85-1452">Ajout de la connexion HTTP à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1452">Added HTTP logging to</span></span> `--debug`

### <a name="acs"></a><span data-ttu-id="a0e85-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1453">ACS</span></span>

* <span data-ttu-id="a0e85-1454">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1454">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a0e85-1455">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1455">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a0e85-1456">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1456">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to</span></span> `aks install-connector`
* <span data-ttu-id="a0e85-1457">Suppression de l’avis de dépréciation dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1457">Removed deprecation notice from</span></span> `aks get-versions`

### <a name="appservice"></a><span data-ttu-id="a0e85-1458">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1458">Appservice</span></span>

* <span data-ttu-id="a0e85-1459">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1459">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a0e85-1460">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="a0e85-1460">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a0e85-1461">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-1461">Cognitive Services</span></span>

* <span data-ttu-id="a0e85-1462">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-1462">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a0e85-1463">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1463">Consumption</span></span>

* <span data-ttu-id="a0e85-1464">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="a0e85-1464">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a0e85-1465">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1465">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1466">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1466">Container</span></span>

* <span data-ttu-id="a0e85-1467">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1467">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1468">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1468">Network</span></span>

* <span data-ttu-id="a0e85-1469">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1469">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in</span></span> `network vnet-gateway vpn-client generate`

### <a name="resource"></a><span data-ttu-id="a0e85-1470">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1470">Resource</span></span>

* <span data-ttu-id="a0e85-1471">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1471">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-1472">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1472">Role</span></span>

* <span data-ttu-id="a0e85-1473">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="a0e85-1473">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1474">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1474">SQL</span></span>

* <span data-ttu-id="a0e85-1475">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1475">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1476">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1476">Storage</span></span>

* <span data-ttu-id="a0e85-1477">Activation de la spécification de préfixe/destination pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1477">Enabled specifying destination-path/prefix for</span></span> `storage blob [upload-batch|download-batch]`

### <a name="vm"></a><span data-ttu-id="a0e85-1478">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1478">VM</span></span>

* <span data-ttu-id="a0e85-1479">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="a0e85-1479">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a0e85-1480">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1480">February 13, 2018</span></span>

<span data-ttu-id="a0e85-1481">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a0e85-1481">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1482">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1482">Core</span></span>

* <span data-ttu-id="a0e85-1483">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1483">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1484">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1484">ACS</span></span>

* <span data-ttu-id="a0e85-1485">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="a0e85-1485">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a0e85-1486">Modification apportée à `aks get-versions` pour afficher les versions Kubernetes disponibles pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1486">Changed `aks get-versions` to show Kubernetes versions available for</span></span> `aks create`
* <span data-ttu-id="a0e85-1487">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1487">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a0e85-1488">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1488">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a0e85-1489">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="a0e85-1489">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a0e85-1490">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1490">Improved reliability when locating the dashboard pod for</span></span> `az aks browse`
* <span data-ttu-id="a0e85-1491">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1491">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a0e85-1492">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1492">Added a message to `az aks install-cli` to help get `kubectl` in</span></span> `$PATH`

### <a name="appservice"></a><span data-ttu-id="a0e85-1493">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1493">Appservice</span></span>

* <span data-ttu-id="a0e85-1494">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="a0e85-1494">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a0e85-1495">Ajout de la prise en charge des plans App Service par défaut via</span><span class="sxs-lookup"><span data-stu-id="a0e85-1495">Added support for default app service plans through</span></span> `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a><span data-ttu-id="a0e85-1496">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-1496">CDN</span></span>

* <span data-ttu-id="a0e85-1497">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1497">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1498">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1498">Container</span></span>

* <span data-ttu-id="a0e85-1499">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="a0e85-1499">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a0e85-1500">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1500">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-1501">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-1501">CosmosDB</span></span>

* <span data-ttu-id="a0e85-1502">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="a0e85-1502">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1503">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1503">Extension</span></span>

* <span data-ttu-id="a0e85-1504">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1504">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a0e85-1505">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1505">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a0e85-1506">Commentaires</span><span class="sxs-lookup"><span data-stu-id="a0e85-1506">Feedback</span></span>

* <span data-ttu-id="a0e85-1507">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="a0e85-1507">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1508">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1508">Interactive</span></span>

* <span data-ttu-id="a0e85-1509">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a0e85-1509">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a0e85-1510">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="a0e85-1510">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-1511">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1511">IoT</span></span>

* <span data-ttu-id="a0e85-1512">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a0e85-1512">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a0e85-1513">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="a0e85-1513">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a0e85-1514">Ajout de la prise en charge de `--no-wait` dans `iot dps access policy [create|update]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1514">Added `--no-wait` support to `iot dps access policy [create|update]` and</span></span> `iot dps linked-hub [create|update]`
* <span data-ttu-id="a0e85-1515">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="a0e85-1515">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1516">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1516">Monitor</span></span>

* <span data-ttu-id="a0e85-1517">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1517">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1518">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1518">Network</span></span>

* <span data-ttu-id="a0e85-1519">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1519">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a0e85-1520">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1520">Profile</span></span>

* <span data-ttu-id="a0e85-1521">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="a0e85-1521">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1522">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1522">Resource</span></span>

* <span data-ttu-id="a0e85-1523">Rajout de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1523">Added back</span></span> `feature show`

### <a name="role"></a><span data-ttu-id="a0e85-1524">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1524">Role</span></span>

* <span data-ttu-id="a0e85-1525">Ajout de l’argument `--available-to-other-tenants` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1525">Added `--available-to-other-tenants` argument to</span></span> `ad app update`

### <a name="sql"></a><span data-ttu-id="a0e85-1526">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1526">SQL</span></span>

* <span data-ttu-id="a0e85-1527">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1527">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a0e85-1528">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-1528">Added</span></span> `sql db rename`
* <span data-ttu-id="a0e85-1529">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="a0e85-1529">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1530">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1530">Storage</span></span>

* <span data-ttu-id="a0e85-1531">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="a0e85-1531">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1532">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1532">VM</span></span>

* <span data-ttu-id="a0e85-1533">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1533">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a0e85-1534">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1534">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a0e85-1535">Résolution</span><span class="sxs-lookup"><span data-stu-id="a0e85-1535">Fixed</span></span> `vm boot-diagnostics get-boot-log`


## <a name="january-31-2018"></a><span data-ttu-id="a0e85-1536">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1536">January 31, 2018</span></span>

<span data-ttu-id="a0e85-1537">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a0e85-1537">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1538">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1538">Core</span></span>

* <span data-ttu-id="a0e85-1539">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1539">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a0e85-1540">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-1540">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a0e85-1541">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1541">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a0e85-1542">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="a0e85-1542">Use `--verbose` to see</span></span>
* <span data-ttu-id="a0e85-1543">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="a0e85-1543">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1544">ACS</span></span>

* <span data-ttu-id="a0e85-1545">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1545">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a0e85-1546">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1546">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1547">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1547">Appservice</span></span>

* <span data-ttu-id="a0e85-1548">Résolution</span><span class="sxs-lookup"><span data-stu-id="a0e85-1548">Fixed</span></span> `webapp log [tail|download]`
* <span data-ttu-id="a0e85-1549">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="a0e85-1549">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a0e85-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-1550">CDN</span></span>

* <span data-ttu-id="a0e85-1551">Résolution du problème de client manquant avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1551">Fixed missing client issue with</span></span> `cdn custom-domain create`

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-1552">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-1552">CosmosDB</span></span>

* <span data-ttu-id="a0e85-1553">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1553">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1554">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1554">Interactive</span></span>

* <span data-ttu-id="a0e85-1555">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="a0e85-1555">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1556">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1556">Network</span></span>

* <span data-ttu-id="a0e85-1557">Ajout de la protection pour `--cert-password` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1557">Added protection for `--cert-password` to</span></span> `application-gateway create`
* <span data-ttu-id="a0e85-1558">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1558">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a0e85-1559">Ajout de la protection pour `--shared-key` et `--authorization-key` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1559">Added protection for `--shared-key` and `--authorization-key` to</span></span> `vpn-connection create`
* <span data-ttu-id="a0e85-1560">Résolution du problème de client manquant avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1560">Fixed missing client issue with</span></span> `asg create`
* <span data-ttu-id="a0e85-1561">Ajout du paramètre `--file-name / -f` pour les noms exportés à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1561">Added `--file-name / -f` parameter for exported names to</span></span> `dns zone export`
* <span data-ttu-id="a0e85-1562">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="a0e85-1562">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a0e85-1563">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1563">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a0e85-1564">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1564">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a0e85-1565">Résolution du problème où certains enregistrements étaient importés deux fois avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1565">Fixed issue where certain records were imported twice with</span></span> `dns zone import`
* <span data-ttu-id="a0e85-1566">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1566">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a0e85-1567">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1567">Profile</span></span>

* <span data-ttu-id="a0e85-1568">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="a0e85-1568">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1569">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1569">Resource</span></span>

* <span data-ttu-id="a0e85-1570">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="a0e85-1570">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1571">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1571">Storage</span></span>

* <span data-ttu-id="a0e85-1572">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="a0e85-1572">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a0e85-1573">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1573">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a0e85-1574">Résolution du bogue empêchant l’utilisation de l’option d’argument « -n » avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1574">Fixed bug preventing "-n" arg option with</span></span> `storage account check-name`
* <span data-ttu-id="a0e85-1575">Ajout de la colonne « snapshot » à la sortie de table pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1575">Added 'snapshot' column to table output for</span></span> `blob [list|show]`
* <span data-ttu-id="a0e85-1576">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="a0e85-1576">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1577">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1577">VM</span></span>

* <span data-ttu-id="a0e85-1578">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="a0e85-1578">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a0e85-1579">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1579">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a0e85-1580">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="a0e85-1580">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a0e85-1581">Ajout de la protection pour `--admin-password` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1581">Added protection for `--admin-password` to</span></span> `[vm|vmss] create`


## <a name="january-17-2018"></a><span data-ttu-id="a0e85-1582">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="a0e85-1582">January 17, 2018</span></span>

<span data-ttu-id="a0e85-1583">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a0e85-1583">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1584">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1584">ACR</span></span>

* <span data-ttu-id="a0e85-1585">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-1585">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a0e85-1586">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="a0e85-1586">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1587">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1587">ACS</span></span>

* <span data-ttu-id="a0e85-1588">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1588">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a0e85-1589">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="a0e85-1589">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1590">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1590">Appservice</span></span>

* <span data-ttu-id="a0e85-1591">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="a0e85-1591">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a0e85-1592">Ajout de la prise en charge des URL personnalisées pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1592">Added support for custom URLs to</span></span> `browse`
* <span data-ttu-id="a0e85-1593">Correction de la prise en charge de l’emplacement pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1593">Fixed slot support for</span></span> `log tail`

### <a name="backup"></a><span data-ttu-id="a0e85-1594">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a0e85-1594">Backup</span></span>

* <span data-ttu-id="a0e85-1595">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="a0e85-1595">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a0e85-1596">Ajout d’options de compte de stockage à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1596">Added storage account options to</span></span> `backup restore restore-disks`
* <span data-ttu-id="a0e85-1597">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-1597">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a0e85-1598">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="a0e85-1598">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a0e85-1599">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1599">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-1600">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1600">Batch</span></span>

* <span data-ttu-id="a0e85-1601">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="a0e85-1601">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a0e85-1602">Cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-1602">Cloud</span></span>

* <span data-ttu-id="a0e85-1603">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-1603">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a0e85-1604">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1604">Consumption</span></span>

* <span data-ttu-id="a0e85-1605">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1605">Added new commands for reservations: `consumption reservations summaries` and</span></span> `consumption reservations details`

### <a name="event-grid"></a><span data-ttu-id="a0e85-1606">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0e85-1606">Event Grid</span></span>

* <span data-ttu-id="a0e85-1607">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers</span><span class="sxs-lookup"><span data-stu-id="a0e85-1607">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="a0e85-1608">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers</span><span class="sxs-lookup"><span data-stu-id="a0e85-1608">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="a0e85-1609">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1609">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a0e85-1610">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="a0e85-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a0e85-1611">Ajout de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1611">Added command</span></span> `eventgrid topic update`
* <span data-ttu-id="a0e85-1612">Ajout de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1612">Added command</span></span> `eventgrid event-subscription update`
* <span data-ttu-id="a0e85-1613">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1613">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a0e85-1614">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="a0e85-1614">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-1615">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-1615">Interactive</span></span>

* <span data-ttu-id="a0e85-1616">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="a0e85-1616">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a0e85-1617">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1617">Fixed errors on startup</span></span>
* <span data-ttu-id="a0e85-1618">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="a0e85-1618">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-1619">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1619">IoT</span></span>

* <span data-ttu-id="a0e85-1620">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="a0e85-1620">Added support for device provisioning service</span></span>
* <span data-ttu-id="a0e85-1621">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1621">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a0e85-1622">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1622">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1623">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1623">Monitor</span></span>

* <span data-ttu-id="a0e85-1624">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1624">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a0e85-1625">Le paramètre `--name` est désormais obligatoire pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1625">The `--name` parameter is now required for</span></span> `az monitor diagnostic-settings create`
* <span data-ttu-id="a0e85-1626">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="a0e85-1626">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1627">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1627">Network</span></span>

* <span data-ttu-id="a0e85-1628">Résolution du problème se produisant lors de la tentative de passage du mode actif au mode de secours, ou inversement, avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1628">Fixed issue when trying to change to/from active-standby mode with</span></span> `vnet-gateway update`
* <span data-ttu-id="a0e85-1629">Ajout de la prise en charge de HTTP2 dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1629">Added support for HTTP2 to</span></span> `application-gateway [create|update]`

### <a name="profile"></a><span data-ttu-id="a0e85-1630">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1630">Profile</span></span>

* <span data-ttu-id="a0e85-1631">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1631">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-1632">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1632">Role</span></span>

* <span data-ttu-id="a0e85-1633">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="a0e85-1633">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0e85-1634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0e85-1634">Service Fabric</span></span>

* <span data-ttu-id="a0e85-1635">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="a0e85-1635">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a0e85-1636">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1636">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1637">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1637">VM</span></span>

* <span data-ttu-id="a0e85-1638">[PRÉVERSION] Prise en charge interzone pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1638">[PREVIEW] Cross-zone support for</span></span> `vmss`
* <span data-ttu-id="a0e85-1639">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="a0e85-1639">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a0e85-1640">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1640">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a0e85-1641">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1641">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a0e85-1642">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="a0e85-1642">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a0e85-1643">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1643">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to</span></span> `[vm|vmss] create`
* <span data-ttu-id="a0e85-1644">Correction des problèmes d’erreur avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1644">Fixed error issues with</span></span> `[vm|vmss] create`
* <span data-ttu-id="a0e85-1645">Correction de l’utilisation excessive des ressources due à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1645">Fixed excessive resource usage caused by</span></span> `vm image list --all`

## <a name="december-19-2017"></a><span data-ttu-id="a0e85-1646">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1646">December 19, 2017</span></span>

<span data-ttu-id="a0e85-1647">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a0e85-1647">Version 2.0.23</span></span>

* <span data-ttu-id="a0e85-1648">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1648">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1649">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1649">Container</span></span>

* <span data-ttu-id="a0e85-1650">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1650">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1651">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1651">Network</span></span>

* <span data-ttu-id="a0e85-1652">Ajout de l’argument `--disable-bgp-route-propagation` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1652">Added `--disable-bgp-route-propagation` argument to</span></span> `route-table [create|update]`
* <span data-ttu-id="a0e85-1653">Ajout de l’argument `--ip-tags` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1653">Added `--ip-tags` argument to</span></span> `public-ip [create|update]`

### <a name="storage"></a><span data-ttu-id="a0e85-1654">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1654">Storage</span></span>

* <span data-ttu-id="a0e85-1655">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="a0e85-1655">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1656">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1656">VM</span></span>

* <span data-ttu-id="a0e85-1657">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1657">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a0e85-1658">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1658">December 5, 2017</span></span>

<span data-ttu-id="a0e85-1659">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a0e85-1659">Version 2.0.22</span></span>

* <span data-ttu-id="a0e85-1660">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1660">Removed `az component` commands.</span></span> <span data-ttu-id="a0e85-1661">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="a0e85-1661">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1662">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1662">Core</span></span>
* <span data-ttu-id="a0e85-1663">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="a0e85-1663">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a0e85-1664">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1664">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1665">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1665">ACS</span></span>

* <span data-ttu-id="a0e85-1666">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1666">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a0e85-1667">Amélioration des rapports d’erreurs pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1667">Improved error reporting for</span></span> `acs create`
* <span data-ttu-id="a0e85-1668">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="a0e85-1668">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a0e85-1669">Advisor</span><span class="sxs-lookup"><span data-stu-id="a0e85-1669">Advisor</span></span>

* <span data-ttu-id="a0e85-1670">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1670">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1671">Appservice</span></span>

* <span data-ttu-id="a0e85-1672">Correction de la génération du nom de certificat avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1672">Fixed cert name generation with</span></span> `webapp config ssl upload`
* <span data-ttu-id="a0e85-1673">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1673">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a0e85-1674">Ajout de la valeur par défaut pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1674">Added default value for</span></span> `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a><span data-ttu-id="a0e85-1675">Consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1675">Consumption</span></span>

* <span data-ttu-id="a0e85-1676">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="a0e85-1676">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1677">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1677">Container</span></span>

* <span data-ttu-id="a0e85-1678">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1678">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1679">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1679">Monitor</span></span>

* <span data-ttu-id="a0e85-1680">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="a0e85-1680">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1681">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1681">Resource</span></span>

* <span data-ttu-id="a0e85-1682">Ajout de l’argument `--include-response-body` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1682">Added `--include-response-body` argument to</span></span> `resource show`

### <a name="role"></a><span data-ttu-id="a0e85-1683">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1683">Role</span></span>

* <span data-ttu-id="a0e85-1684">Ajout de l’affichage des attributions par défaut pour les administrateurs « classiques » à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1684">Added display of default assignments for "classic" administraors to</span></span> `role assignment list`
* <span data-ttu-id="a0e85-1685">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1685">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a0e85-1686">Amélioration des rapports d’erreurs pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1686">Improved error reporting for</span></span> `ad sp create-for-rbac`

### <a name="sql"></a><span data-ttu-id="a0e85-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1687">SQL</span></span>

* <span data-ttu-id="a0e85-1688">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1688">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a0e85-1689">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1689">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1690">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1690">VM</span></span>

* <span data-ttu-id="a0e85-1691">Ajout des informations de zone à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1691">Added zone information to</span></span> `az vm list-skus`


## <a name="november-14-2017"></a><span data-ttu-id="a0e85-1692">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1692">November 14, 2017</span></span>

<span data-ttu-id="a0e85-1693">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a0e85-1693">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-1694">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1694">ACR</span></span>

* <span data-ttu-id="a0e85-1695">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="a0e85-1695">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a0e85-1696">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1696">ACS</span></span>

* <span data-ttu-id="a0e85-1697">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1697">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a0e85-1698">Option `--orchestrator-release` dépréciée pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1698">Deprecated `--orchestrator-release` option for</span></span> `acs create`
* <span data-ttu-id="a0e85-1699">Changement de la taille de machine virtuelle par défaut pour AKS à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1699">Changed default VM size for AKS to</span></span> `Standard_D1_v2`
* <span data-ttu-id="a0e85-1700">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-1700">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a0e85-1701">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="a0e85-1701">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1702">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1702">Appservice</span></span>

* <span data-ttu-id="a0e85-1703">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="a0e85-1703">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a0e85-1704">Ajout de l’option `--docker-container-logging` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1704">Added `--docker-container-logging` option to</span></span> `az webapp log config`
* <span data-ttu-id="a0e85-1705">Suppression de l’option `storage` pour le paramètre `--web-server-logging` de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1705">Removed the `storage` option from the parameter `--web-server-logging` of</span></span> `az webapp log config`
* <span data-ttu-id="a0e85-1706">Amélioration des messages d’erreur pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1706">Improved error messages for</span></span> `deployment user set`
* <span data-ttu-id="a0e85-1707">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="a0e85-1707">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a0e85-1708">Résolution</span><span class="sxs-lookup"><span data-stu-id="a0e85-1708">Fixed</span></span> `list-locations`

### <a name="batch"></a><span data-ttu-id="a0e85-1709">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1709">Batch</span></span>

* <span data-ttu-id="a0e85-1710">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1710">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a0e85-1711">Batchai</span><span class="sxs-lookup"><span data-stu-id="a0e85-1711">Batchai</span></span>

* <span data-ttu-id="a0e85-1712">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1712">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a0e85-1713">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1713">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a0e85-1714">Correction de la documentation pour `job list-files` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1714">Fixed documentation for `job list-files` and</span></span> `job stream-file`
* <span data-ttu-id="a0e85-1715">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1715">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a0e85-1716">Cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-1716">Cloud</span></span>

* <span data-ttu-id="a0e85-1717">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="a0e85-1717">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1718">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1718">Container</span></span>

* <span data-ttu-id="a0e85-1719">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="a0e85-1719">Added support to open multiple ports</span></span>
* <span data-ttu-id="a0e85-1720">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1720">Added container group restart policy</span></span>
* <span data-ttu-id="a0e85-1721">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="a0e85-1721">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a0e85-1722">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="a0e85-1722">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0e85-1723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0e85-1723">Data Lake Analytics</span></span>

* <span data-ttu-id="a0e85-1724">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a0e85-1724">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a0e85-1725">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-1725">Data Lake Store</span></span>

* <span data-ttu-id="a0e85-1726">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="a0e85-1726">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a0e85-1727">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1727">Extension</span></span>

* <span data-ttu-id="a0e85-1728">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="a0e85-1728">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a0e85-1729">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="a0e85-1729">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-1730">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1730">IoT</span></span>

* <span data-ttu-id="a0e85-1731">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1731">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1732">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1732">Monitor</span></span>

* <span data-ttu-id="a0e85-1733">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1733">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1734">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1734">Network</span></span>

* <span data-ttu-id="a0e85-1735">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="a0e85-1735">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a0e85-1736">Résolution d’un problème empêchant la mise à jour des points de terminaison avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1736">Fixed issue where endpoints could not be updated with</span></span> `traffic-manager profile update`
* <span data-ttu-id="a0e85-1737">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="a0e85-1737">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a0e85-1738">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par</span><span class="sxs-lookup"><span data-stu-id="a0e85-1738">Fixed issue where relative DNS names were incorrectly imported by</span></span> `dns zone import`

### <a name="reservations"></a><span data-ttu-id="a0e85-1739">Réservations</span><span class="sxs-lookup"><span data-stu-id="a0e85-1739">Reservations</span></span>

* <span data-ttu-id="a0e85-1740">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1740">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1741">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1741">Resource</span></span>

* <span data-ttu-id="a0e85-1742">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a0e85-1742">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1743">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1743">SQL</span></span>

* <span data-ttu-id="a0e85-1744">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1744">Added `--ignore-missing-vnet-service-endpoint` parameter to</span></span> `sql server vnet-rule [create|update]`

### <a name="storage"></a><span data-ttu-id="a0e85-1745">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1745">Storage</span></span>

* <span data-ttu-id="a0e85-1746">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-1746">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a0e85-1747">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="a0e85-1747">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a0e85-1748">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1748">Fixed bug that prevented using `--source-uri` with</span></span> `storage [blob|file] copy start-batch`
* <span data-ttu-id="a0e85-1749">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1749">Added commands to glob and delete multiple objects with</span></span> `storage [blob|file] delete-batch`
* <span data-ttu-id="a0e85-1750">Résolution du problème de l’activation des métriques avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1750">Fixed issue when enabling metrics with</span></span> `storage metrics update`
* <span data-ttu-id="a0e85-1751">Résolution du problème avec les fichiers de plus de 200 Go lors de l’utilisation de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1751">Fixed issue with files over 200GB when using</span></span> `storage blob upload-batch`
* <span data-ttu-id="a0e85-1752">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par</span><span class="sxs-lookup"><span data-stu-id="a0e85-1752">Fixed issue where `--bypass` and `--default-action` were ignored by</span></span> `storage account [create|update]`

### <a name="vm"></a><span data-ttu-id="a0e85-1753">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1753">VM</span></span>

* <span data-ttu-id="a0e85-1754">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1754">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a0e85-1755">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1755">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a0e85-1756">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="a0e85-1756">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a0e85-1757">Renommage de `vm format-secret` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1757">Renamed `vm format-secret` to</span></span> `vm secret format`
* <span data-ttu-id="a0e85-1758">Ajout de l’argument `--encrypt format` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1758">Added `--encrypt format` argument to</span></span> `vm encryption enable`

## <a name="october-24-2017"></a><span data-ttu-id="a0e85-1759">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1759">October 24, 2017</span></span>

<span data-ttu-id="a0e85-1760">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a0e85-1760">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1761">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1761">Core</span></span>

* <span data-ttu-id="a0e85-1762">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version</span><span class="sxs-lookup"><span data-stu-id="a0e85-1762">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version</span></span> `2016-01-01`

### <a name="acr"></a><span data-ttu-id="a0e85-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-1763">ACR</span></span>

* <span data-ttu-id="a0e85-1764">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1764">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a0e85-1765">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="a0e85-1765">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a0e85-1766">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="a0e85-1766">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1767">ACS</span></span>

* <span data-ttu-id="a0e85-1768">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1768">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a0e85-1769">Correction de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1769">Fixed kubernetes</span></span> `get-credentials`

### <a name="appservice"></a><span data-ttu-id="a0e85-1770">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1770">Appservice</span></span>

* <span data-ttu-id="a0e85-1771">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="a0e85-1771">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a0e85-1772">Composant</span><span class="sxs-lookup"><span data-stu-id="a0e85-1772">Component</span></span>

* <span data-ttu-id="a0e85-1773">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1773">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-1774">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-1774">Monitor</span></span>

* <span data-ttu-id="a0e85-1775">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1775">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1776">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1776">Resource</span></span>

* <span data-ttu-id="a0e85-1777">Résolution d’une incompatibilité avec la dernière version de la dépendance msrest dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1777">Fixed incompatibility with most recent version of msrest dependency in</span></span> `group export`
* <span data-ttu-id="a0e85-1778">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1778">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1779">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1779">VM</span></span>

* <span data-ttu-id="a0e85-1780">Ajout de l’argument `--accelerated-networking` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1780">Added `--accelerated-networking` argument to</span></span> `vmss create`


## <a name="october-9-2017"></a><span data-ttu-id="a0e85-1781">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1781">October 9, 2017</span></span>

<span data-ttu-id="a0e85-1782">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a0e85-1782">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1783">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1783">Core</span></span>

* <span data-ttu-id="a0e85-1784">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a0e85-1784">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1785">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1785">Appservice</span></span>

* <span data-ttu-id="a0e85-1786">Ajout de la mise à jour générique avec la nouvelle commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1786">Added generic update with new command</span></span> `webapp update`

### <a name="batch"></a><span data-ttu-id="a0e85-1787">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1787">Batch</span></span>

* <span data-ttu-id="a0e85-1788">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a0e85-1788">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a0e85-1789">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="a0e85-1789">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a0e85-1790">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1790">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a0e85-1791">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="a0e85-1791">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a0e85-1792">Batchai</span><span class="sxs-lookup"><span data-stu-id="a0e85-1792">Batchai</span></span>

* <span data-ttu-id="a0e85-1793">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="a0e85-1793">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-1794">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-1794">Keyvault</span></span>

* <span data-ttu-id="a0e85-1795">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1795">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a0e85-1796">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1796">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a0e85-1797">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1797">Network</span></span>

* <span data-ttu-id="a0e85-1798">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="a0e85-1798">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a0e85-1799">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1799">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1800">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1800">Resource</span></span>

* <span data-ttu-id="a0e85-1801">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1801">Added support for `--resource-group/-g` options for resource group name to</span></span> `group`
* <span data-ttu-id="a0e85-1802">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1802">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a0e85-1803">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="a0e85-1803">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a0e85-1804">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="a0e85-1804">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1805">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1805">Sql</span></span>

* <span data-ttu-id="a0e85-1806">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="a0e85-1806">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a0e85-1807">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="a0e85-1807">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a0e85-1808">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="a0e85-1808">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1809">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1809">Storage</span></span>

* <span data-ttu-id="a0e85-1810">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="a0e85-1810">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1811">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1811">Vm</span></span>

* <span data-ttu-id="a0e85-1812">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1812">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a0e85-1813">[PRÉVERSION] Ajout de la prise en charge de la mise à niveau propagée pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1813">[PREVIEW] Added support for rolling upgrade to</span></span> `vmss create`
* <span data-ttu-id="a0e85-1814">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1814">Added support for updating encryption settings with</span></span> `vm encryption enable`
* <span data-ttu-id="a0e85-1815">Ajout du paramètre `--os-disk-size-gb` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1815">Added `--os-disk-size-gb` parameter to</span></span> `vm create`
* <span data-ttu-id="a0e85-1816">Ajout du paramètre `--license-type` pour Windows dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1816">Added `--license-type` parameter for Windows to</span></span> `vmss create`


## <a name="september-22-2017"></a><span data-ttu-id="a0e85-1817">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1817">September 22, 2017</span></span>

<span data-ttu-id="a0e85-1818">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a0e85-1818">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-1819">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1819">Resource</span></span>

* <span data-ttu-id="a0e85-1820">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1820">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a0e85-1821">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="a0e85-1821">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a0e85-1822">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1822">Added support for UI definitions and templates to</span></span> `managedapp definition create`
* <span data-ttu-id="a0e85-1823">[CHANGEMENT CASSANT] Changement du type de ressource `managedapp` de `appliances` en `applications` et `applianceDefinitions` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-1823">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to</span></span> `applicationDefinitions`

### <a name="network"></a><span data-ttu-id="a0e85-1824">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1824">Network</span></span>

* <span data-ttu-id="a0e85-1825">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1825">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a0e85-1826">Ajout de la prise en charge de l’appairage Microsoft IPv6 pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1826">Added support for IPv6 Microsoft Peering to</span></span> `express-route`
* <span data-ttu-id="a0e85-1827">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1827">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a0e85-1828">Ajout de l’argument `--application-security-groups` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1828">Added `--application-security-groups` argument to</span></span> `nic [create|ip-config create|ip-config update]`
* <span data-ttu-id="a0e85-1829">Ajout des arguments `--source-asgs` et `--destination-asgs` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1829">Added `--source-asgs` and `--destination-asgs` arguments to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="a0e85-1830">Ajout des arguments `--ddos-protection` et `--vm-protection` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1830">Added `--ddos-protection` and `--vm-protection` arguments to</span></span> `vnet [create|update]`
* <span data-ttu-id="a0e85-1831">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1831">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1832">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1832">Storage</span></span>

* <span data-ttu-id="a0e85-1833">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1833">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a0e85-1834">Événement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1834">Eventgrid</span></span>

* <span data-ttu-id="a0e85-1835">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="a0e85-1835">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1836">SQL</span></span>

* <span data-ttu-id="a0e85-1837">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1837">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a0e85-1838">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1838">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a0e85-1839">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1839">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and</span></span> `dw [create|update]`

### <a name="keyvault"></a><span data-ttu-id="a0e85-1840">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-1840">Keyvault</span></span>

* <span data-ttu-id="a0e85-1841">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="a0e85-1841">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1842">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1842">VM</span></span>

* <span data-ttu-id="a0e85-1843">Ajout de la prise en charge de zone de disponibilité pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1843">Added for support to availability zone to</span></span> `[vm|vmss|disk] create`
* <span data-ttu-id="a0e85-1844">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1844">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a0e85-1845">Ajout de l’argument `--asgs` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1845">Added `--asgs` argument to</span></span> `vm create`
* <span data-ttu-id="a0e85-1846">Ajout de la prise en charge de l’exécution de commandes sur des machines virtuelles avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1846">Added support for running commands on VMs with</span></span> `vm run-command`
* <span data-ttu-id="a0e85-1847">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1847">[PREVIEW] Added support for VMSS disk encryption with</span></span> `vmss encryption`
* <span data-ttu-id="a0e85-1848">Ajout de la prise en charge de la maintenance sur des machines virtuelles avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1848">Added support for performing maintenance on VMs with</span></span> `vm perform-maintenance`

### <a name="acs"></a><span data-ttu-id="a0e85-1849">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1849">ACS</span></span>

* <span data-ttu-id="a0e85-1850">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="a0e85-1850">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1851">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1851">Appservice</span></span>

* <span data-ttu-id="a0e85-1852">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1852">Added ability to update and show authentication settings with</span></span> `webapp auth [update|show]`

### <a name="backup"></a><span data-ttu-id="a0e85-1853">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="a0e85-1853">Backup</span></span>

* <span data-ttu-id="a0e85-1854">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-1854">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a0e85-1855">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1855">September 11, 2017</span></span>

<span data-ttu-id="a0e85-1856">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a0e85-1856">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a0e85-1857">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1857">Core</span></span>

* <span data-ttu-id="a0e85-1858">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="a0e85-1858">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a0e85-1859">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="a0e85-1859">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1860">Acs</span><span class="sxs-lookup"><span data-stu-id="a0e85-1860">Acs</span></span>

* <span data-ttu-id="a0e85-1861">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1861">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a0e85-1862">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="a0e85-1862">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1863">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1863">Appservice</span></span>

* <span data-ttu-id="a0e85-1864">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="a0e85-1864">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a0e85-1865">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-1865">CDN</span></span>

* <span data-ttu-id="a0e85-1866">Correction du bogue « CustomDomain n’est pas itérable » pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1866">Fixed 'CustomDomain is not interable' bug for</span></span> `cdn custom-domain create`

### <a name="extension"></a><span data-ttu-id="a0e85-1867">Extension</span><span class="sxs-lookup"><span data-stu-id="a0e85-1867">Extension</span></span>

* <span data-ttu-id="a0e85-1868">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1868">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-1869">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-1869">Keyvault</span></span>

* <span data-ttu-id="a0e85-1870">Résolution du problème de respect de la casse au niveau des autorisations pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1870">Fixed issue where permissions were case sensitive for</span></span> `keyvault set-policy`

### <a name="network"></a><span data-ttu-id="a0e85-1871">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1871">Network</span></span>

* <span data-ttu-id="a0e85-1872">Renommage de `vnet list-private-access-services` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1872">Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="a0e85-1873">Renommage de l’argument `--private-access-services` en `--service-endpoints` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1873">Renamed `--private-access-services` argument to `--service-endpoints` for</span></span> `vnet subnet create/update`
* <span data-ttu-id="a0e85-1874">Ajout de la prise en charge de plusieurs plages IP et de ports à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1874">Added support for multiple IP ranges and port ranges to</span></span> `nsg rule create/update`
* <span data-ttu-id="a0e85-1875">Ajout de la prise en charge de la référence SKU pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1875">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="a0e85-1876">Ajout de la prise en charge de la référence SKU pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1876">Added support for SKU to</span></span> `public-ip create`

### <a name="resource"></a><span data-ttu-id="a0e85-1877">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-1877">Resource</span></span>

* <span data-ttu-id="a0e85-1878">Autoriser le passage des définitions de paramètres de stratégie de ressource dans `policy definition create`, et</span><span class="sxs-lookup"><span data-stu-id="a0e85-1878">Allow passing in resource policy parameter definitions in `policy definition create`, and</span></span> `policy definition update`
* <span data-ttu-id="a0e85-1879">Autoriser le passage des valeurs de paramètres pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1879">Allow passing in parameter values for</span></span> `policy assignment create`
* <span data-ttu-id="a0e85-1880">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="a0e85-1880">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a0e85-1881">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="a0e85-1881">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-1882">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-1882">SQL</span></span>

* <span data-ttu-id="a0e85-1883">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1883">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1884">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1884">VM</span></span>

* <span data-ttu-id="a0e85-1885">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="a0e85-1885">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a0e85-1886">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1886">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a0e85-1887">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1887">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a0e85-1888">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="a0e85-1888">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a0e85-1889">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="a0e85-1889">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a0e85-1890">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1890">August 31, 2017</span></span>

<span data-ttu-id="a0e85-1891">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a0e85-1891">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-1892">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-1892">Keyvault</span></span>

* <span data-ttu-id="a0e85-1893">Correction d’un bogue qui se produit lors de la tentative de résolution automatique de l’encodage secret avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1893">Fixed bug when trying to automatically resolve secret encoding with</span></span> `secret download`

### <a name="sf"></a><span data-ttu-id="a0e85-1894">Sf</span><span class="sxs-lookup"><span data-stu-id="a0e85-1894">Sf</span></span>

* <span data-ttu-id="a0e85-1895">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1895">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1896">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1896">Storage</span></span>

* <span data-ttu-id="a0e85-1897">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="a0e85-1897">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a0e85-1898">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="a0e85-1898">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a0e85-1899">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1899">August 28, 2017</span></span>

<span data-ttu-id="a0e85-1900">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a0e85-1900">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a0e85-1901">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1901">CLI</span></span>

* <span data-ttu-id="a0e85-1902">Ajout d’une remarque juridique pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1902">Added legal note to</span></span> `--version`

### <a name="acs"></a><span data-ttu-id="a0e85-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1903">ACS</span></span>

* <span data-ttu-id="a0e85-1904">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a0e85-1904">Corrected preview regions</span></span>
* <span data-ttu-id="a0e85-1905">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1905">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a0e85-1906">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1906">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1907">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1907">Appservice</span></span>

* <span data-ttu-id="a0e85-1908">[CHANGEMENT CASSANT] Correction des incohérences dans la sortie de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1908">[BREAKING CHANGE] Fixed inconsistencies in the output of</span></span> `az webapp config appsettings [delete|set]`
* <span data-ttu-id="a0e85-1909">Ajout d’un nouvel alias de `-i` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1909">Added a new alias of `-i` for</span></span> `az webapp config container set --docker-custom-image-name`
* <span data-ttu-id="a0e85-1910">Exposé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1910">Exposed</span></span> `az webapp log show`
* <span data-ttu-id="a0e85-1911">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1911">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a0e85-1912">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1912">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-1913">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-1913">IoT</span></span>

* <span data-ttu-id="a0e85-1914">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1914">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1915">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1915">Network</span></span>

* <span data-ttu-id="a0e85-1916">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-1916">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="a0e85-1917">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1917">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for</span></span> `vnet subnet [create|update]`
* <span data-ttu-id="a0e85-1918">Ajout de la prise en charge de plusieurs plages d’IP et de ports pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1918">Added support for multiple IP and port ranges to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="a0e85-1919">Ajout de la prise en charge de la référence SKU pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1919">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="a0e85-1920">Ajout de la prise en charge de la référence SKU pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1920">Added support for SKU to</span></span> `public-ip create`

### <a name="profile"></a><span data-ttu-id="a0e85-1921">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1921">Profile</span></span>

* <span data-ttu-id="a0e85-1922">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1922">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0e85-1923">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0e85-1923">Service Fabric</span></span>

* <span data-ttu-id="a0e85-1924">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-1924">Preview release</span></span>
* <span data-ttu-id="a0e85-1925">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1925">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a0e85-1926">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="a0e85-1926">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a0e85-1927">Ajout de la prise en charge des valeurs vides pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1927">Added support for empty</span></span> `registry_cred`

### <a name="storage"></a><span data-ttu-id="a0e85-1928">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1928">Storage</span></span>

* <span data-ttu-id="a0e85-1929">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1929">Enabled setting blob tier</span></span>
* <span data-ttu-id="a0e85-1930">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="a0e85-1930">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a0e85-1931">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à</span><span class="sxs-lookup"><span data-stu-id="a0e85-1931">Added commands to add VNET rules and IP based rules to</span></span> `storage account network-rule`
* <span data-ttu-id="a0e85-1932">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="a0e85-1932">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a0e85-1933">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1933">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a0e85-1934">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="a0e85-1934">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1935">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1935">VM</span></span>

* <span data-ttu-id="a0e85-1936">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation de</span><span class="sxs-lookup"><span data-stu-id="a0e85-1936">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using</span></span> `--instance-id *`
* <span data-ttu-id="a0e85-1937">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="a0e85-1937">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a0e85-1938">Suppression de noms de personnes de la liste rouge des noms d’administrateur pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-1938">Removed human names from the admin name blacklist for</span></span> `[vm|vmss] create`
* <span data-ttu-id="a0e85-1939">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="a0e85-1939">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a0e85-1940">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="a0e85-1940">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a0e85-1941">Correction d’un problème qui empêchait l’argument `--no-wait` de fonctionner avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1941">Fixed issue where `--no-wait` argument did not work wth</span></span> `vm availability-set create`


## <a name="august-15-2017"></a><span data-ttu-id="a0e85-1942">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1942">August 15, 2017</span></span>

<span data-ttu-id="a0e85-1943">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a0e85-1943">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1944">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1944">ACS</span></span>

* <span data-ttu-id="a0e85-1945">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="a0e85-1945">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-1946">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-1946">Appservice</span></span>

* <span data-ttu-id="a0e85-1947">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="a0e85-1947">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a0e85-1948">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0e85-1948">Event Grid</span></span>

* <span data-ttu-id="a0e85-1949">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1949">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a0e85-1950">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1950">August 11, 2017</span></span>

<span data-ttu-id="a0e85-1951">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a0e85-1951">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-1952">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-1952">ACS</span></span>

* <span data-ttu-id="a0e85-1953">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="a0e85-1953">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a0e85-1954">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-1954">Batch</span></span>

* <span data-ttu-id="a0e85-1955">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a0e85-1955">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a0e85-1956">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1956">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a0e85-1957">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="a0e85-1957">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a0e85-1958">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="a0e85-1958">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a0e85-1959">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="a0e85-1959">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a0e85-1960">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="a0e85-1960">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a0e85-1961">Composant</span><span class="sxs-lookup"><span data-stu-id="a0e85-1961">Component</span></span>

* <span data-ttu-id="a0e85-1962">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="a0e85-1962">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a0e85-1963">Conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1963">Container</span></span>

* `create`<span data-ttu-id="a0e85-1964">: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1964">: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a0e85-1965">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-1965">Data Lake Store</span></span>

* <span data-ttu-id="a0e85-1966">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="a0e85-1966">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a0e85-1967">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a0e85-1967">Event Grid</span></span>

* <span data-ttu-id="a0e85-1968">Version initiale</span><span class="sxs-lookup"><span data-stu-id="a0e85-1968">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-1969">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-1969">Network</span></span>

* `lb`<span data-ttu-id="a0e85-1970">: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="a0e85-1970">: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* `application-gateway {subresource} delete`<span data-ttu-id="a0e85-1971">: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1971">: Fixed issue where `--no-wait` was not honored</span></span>
* `application-gateway http-settings update`<span data-ttu-id="a0e85-1972">: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="a0e85-1972">: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a0e85-1973">Correction de l’erreur liée à l’argument de mot clé inattendu `sa_data_size_kilobyes` avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-1973">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with</span></span> `az network vpn-connection ipsec-policy add`

### <a name="profile"></a><span data-ttu-id="a0e85-1974">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-1974">Profile</span></span>

* `account list`<span data-ttu-id="a0e85-1975">: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1975">: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-1976">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-1976">Storage</span></span>

* <span data-ttu-id="a0e85-1977">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="a0e85-1977">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-1978">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1978">VM</span></span>

* `availability-set`<span data-ttu-id="a0e85-1979">: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="a0e85-1979">: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a0e85-1980">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="a0e85-1980">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a0e85-1981">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-1981">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a0e85-1982">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="a0e85-1982">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a0e85-1983">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="a0e85-1983">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a0e85-1984">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-1984">July 28, 2017</span></span>

<span data-ttu-id="a0e85-1985">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a0e85-1985">Version 2.0.12</span></span>

* <span data-ttu-id="a0e85-1986">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="a0e85-1986">Added container commands</span></span>
* <span data-ttu-id="a0e85-1987">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="a0e85-1987">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a0e85-1988">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-1988">Core</span></span>

* <span data-ttu-id="a0e85-1989">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="a0e85-1989">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a0e85-1990">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1990">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a0e85-1991">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a0e85-1991">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a0e85-1992">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1992">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a0e85-1993">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="a0e85-1993">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a0e85-1994">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1994">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a0e85-1995">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1995">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a0e85-1996">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1996">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a0e85-1997">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1997">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a0e85-1998">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a0e85-1998">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a0e85-1999">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="a0e85-1999">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a0e85-2000">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2000">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a0e85-2001">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-2001">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a0e85-2002">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="a0e85-2002">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a0e85-2003">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a0e85-2003">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a0e85-2004">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2004">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a0e85-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-2005">ACR</span></span>

* <span data-ttu-id="a0e85-2006">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a0e85-2006">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a0e85-2007">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="a0e85-2007">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a0e85-2008">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="a0e85-2008">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a0e85-2009">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="a0e85-2009">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a0e85-2010">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="a0e85-2010">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a0e85-2011">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="a0e85-2011">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-2012">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-2012">ACS</span></span>

* <span data-ttu-id="a0e85-2013">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="a0e85-2013">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-2014">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-2014">Appservice</span></span>

* <span data-ttu-id="a0e85-2015">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="a0e85-2015">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a0e85-2016">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="a0e85-2016">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a0e85-2017">Supprimer toutes les commandes sous</span><span class="sxs-lookup"><span data-stu-id="a0e85-2017">Remove all commands under</span></span> `appservice web`
* <span data-ttu-id="a0e85-2018">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2018">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a0e85-2019">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2019">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a0e85-2020">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2020">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a0e85-2021">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2021">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a0e85-2022">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2022">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a0e85-2023">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2023">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a0e85-2024">Utilisez à la place</span><span class="sxs-lookup"><span data-stu-id="a0e85-2024">Instead use</span></span> `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a><span data-ttu-id="a0e85-2025">Batch</span><span class="sxs-lookup"><span data-stu-id="a0e85-2025">Batch</span></span>

* <span data-ttu-id="a0e85-2026">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="a0e85-2026">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a0e85-2027">Renommage de l’option `pool create` en `--target-dedicated` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-2027">Renamed `pool create` option `--target-dedicated` to</span></span> `--target-dedicated-nodes`
* <span data-ttu-id="a0e85-2028">Ajout des options `pool create` `--target-low-priority-nodes` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2028">Added `pool create` options `--target-low-priority-nodes` and</span></span> `--application-licenses`

### <a name="cdn"></a><span data-ttu-id="a0e85-2029">CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-2029">CDN</span></span>

* <span data-ttu-id="a0e85-2030">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-2030">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a0e85-2031">Cloud</span><span class="sxs-lookup"><span data-stu-id="a0e85-2031">Cloud</span></span>

* <span data-ttu-id="a0e85-2032">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="a0e85-2032">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a0e85-2033">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2033">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a0e85-2034">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="a0e85-2034">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a0e85-2035">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="a0e85-2035">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a0e85-2036">Exposé</span><span class="sxs-lookup"><span data-stu-id="a0e85-2036">Exposed</span></span> `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-2037">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-2037">CosmosDB</span></span>

* <span data-ttu-id="a0e85-2038">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="a0e85-2038">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a0e85-2039">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="a0e85-2039">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0e85-2040">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0e85-2040">Data Lake Analytics</span></span>

* <span data-ttu-id="a0e85-2041">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2041">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a0e85-2042">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-2042">Added</span></span> `dla job pipeline show`
* <span data-ttu-id="a0e85-2043">Ajouté</span><span class="sxs-lookup"><span data-stu-id="a0e85-2043">Added</span></span> `dla job recurrence list`

### <a name="data-lake-store"></a><span data-ttu-id="a0e85-2044">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-2044">Data Lake Store</span></span>

* <span data-ttu-id="a0e85-2045">Ajout de la prise en charge de la rotation des clés de coffre gérées par l’utilisateur dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-2045">Added support for user managed key vault key rotation in</span></span> `dls account update`
* <span data-ttu-id="a0e85-2046">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="a0e85-2046">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a0e85-2047">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2047">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a0e85-2048">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-2048">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a0e85-2049">Interactive</span><span class="sxs-lookup"><span data-stu-id="a0e85-2049">Interactive</span></span>

* <span data-ttu-id="a0e85-2050">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="a0e85-2050">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a0e85-2051">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="a0e85-2051">Increased test coverage</span></span>
* <span data-ttu-id="a0e85-2052">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="a0e85-2052">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a0e85-2053">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2053">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a0e85-2054">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2054">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a0e85-2055">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2055">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a0e85-2056">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2056">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a0e85-2057">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2057">Added `--progress` flag</span></span>
* <span data-ttu-id="a0e85-2058">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="a0e85-2058">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a0e85-2059">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2059">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a0e85-2060">IoT</span><span class="sxs-lookup"><span data-stu-id="a0e85-2060">IoT</span></span>

* <span data-ttu-id="a0e85-2061">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2061">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a0e85-2062">(#3934)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2062">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a0e85-2063">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="a0e85-2063">Key vault</span></span>

* <span data-ttu-id="a0e85-2064">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2064">Added commands for key vault recovery features:</span></span>
  * `keyvault` <span data-ttu-id="a0e85-2065">sous-commandes `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2065">subcommands `purge`, `recover`,</span></span> `keyvault list-deleted`
  * `keyvault secret` <span data-ttu-id="a0e85-2066">sous-commandes `backup`, `restore`, `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2066">subcommands `backup`, `restore`, `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault certificate` <span data-ttu-id="a0e85-2067">sous-commandes `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2067">subcommands `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault key` <span data-ttu-id="a0e85-2068">sous-commandes `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2068">subcommands `purge`, `recover`,</span></span> `list-deleted`
* <span data-ttu-id="a0e85-2069">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2069">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a0e85-2070">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2070">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a0e85-2071">(#3307)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2071">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a0e85-2072">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2072">Lab</span></span>

* <span data-ttu-id="a0e85-2073">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le labo via</span><span class="sxs-lookup"><span data-stu-id="a0e85-2073">Added support for claiming any vm in the lab through</span></span> `az lab vm claim`
* <span data-ttu-id="a0e85-2074">Ajout du formateur de sortie de tableau pour `az lab vm list` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2074">Added table output formatter for `az lab vm list` and</span></span> `az lab vm show`

### <a name="monitor"></a><span data-ttu-id="a0e85-2075">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-2075">Monitor</span></span>

* <span data-ttu-id="a0e85-2076">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2076">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a0e85-2077">Renommage de `monitor alert-rule-incidents list` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-2077">Renamed `monitor alert-rule-incidents list` to</span></span> `monitor alert list-incidents`
* <span data-ttu-id="a0e85-2078">Renommage de `monitor alert-rule-incidents show` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-2078">Renamed `monitor alert-rule-incidents show` to</span></span> `monitor alert show-incident`
* <span data-ttu-id="a0e85-2079">Renommage de `monitor metric-defintions list` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-2079">Renamed `monitor metric-defintions list` to</span></span> `monitor metrics list-definitions`
* <span data-ttu-id="a0e85-2080">Renommage de `monitor alert-rules` en</span><span class="sxs-lookup"><span data-stu-id="a0e85-2080">Renamed `monitor alert-rules` to</span></span> `monitor alert`
* <span data-ttu-id="a0e85-2081">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="a0e85-2081">Changed `monitor alert create`:</span></span>
  * `condition` <span data-ttu-id="a0e85-2082">et la sous-commande `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="a0e85-2082">and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a0e85-2083">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2083">Add numerous parameters to simplify the rule creation process</span></span>
  * `location` <span data-ttu-id="a0e85-2084">n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2084">no longer required</span></span>
  * <span data-ttu-id="a0e85-2085">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="a0e85-2085">Add name and ID support for target</span></span>
  * <span data-ttu-id="a0e85-2086">Supprimer</span><span class="sxs-lookup"><span data-stu-id="a0e85-2086">Remove</span></span> `--alert-rule-resource-name`
  * <span data-ttu-id="a0e85-2087">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2087">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * `description` <span data-ttu-id="a0e85-2088">sont désormais basées par défaut sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="a0e85-2088">defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a0e85-2089">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="a0e85-2089">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a0e85-2090">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2090">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a0e85-2091">Ajout d’arguments d’usage et d’exemples pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-2091">Added convenience arguments and examples to</span></span> `monitor alert rule update`

### <a name="network"></a><span data-ttu-id="a0e85-2092">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-2092">Network</span></span>

* <span data-ttu-id="a0e85-2093">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2093">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a0e85-2094">Ajout de l’argument `--private-access-services` à `vnet subnet create` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2094">Added `--private-access-services` argument to `vnet subnet create` and</span></span> `vnet subnet update`
* <span data-ttu-id="a0e85-2095">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="a0e85-2095">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a0e85-2096">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="a0e85-2096">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a0e85-2097">Correction d’un bogue lié à l’utilisation de l’argument `--servers` avec `application-gateway address-pool create` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2097">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and</span></span> `application-gateway address-pool update`
* <span data-ttu-id="a0e85-2098">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2098">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a0e85-2099">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2099">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`,</span></span> `predefined show`
* <span data-ttu-id="a0e85-2100">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2100">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span></span> `--min-protocol-version`
* <span data-ttu-id="a0e85-2101">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2101">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a0e85-2102">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update` : `--default-redirect-config`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2102">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`,</span></span> `--redirect-config`
* <span data-ttu-id="a0e85-2103">Ajout de l’argument `--redirect-config` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-2103">Added argument `--redirect-config` to</span></span> `application-gateway url-path-map rule create`
* <span data-ttu-id="a0e85-2104">Ajout de la prise en charge de `--no-wait` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-2104">Added support for `--no-wait` to</span></span> `application-gateway url-path-map rule delete`
* <span data-ttu-id="a0e85-2105">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span><span class="sxs-lookup"><span data-stu-id="a0e85-2105">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span></span> `--match-status-codes`
* <span data-ttu-id="a0e85-2106">Ajout de l’argument `--redirect-config` à `application-gateway rule create` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2106">Added argument `--redirect-config` to `application-gateway rule create` and</span></span> `application-gateway rule update`
* <span data-ttu-id="a0e85-2107">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2107">Added support for `--accelerated-networking` to `nic create` and</span></span> `nic update`
* <span data-ttu-id="a0e85-2108">Suppression de l’argument `--internal-dns-name-suffix` dans</span><span class="sxs-lookup"><span data-stu-id="a0e85-2108">Removed `--internal-dns-name-suffix` argument from</span></span> `nic create`
* <span data-ttu-id="a0e85-2109">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="a0e85-2109">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a0e85-2110">Correction d’un bogue où `local-gateway create` était ignoré</span><span class="sxs-lookup"><span data-stu-id="a0e85-2110">Fixed bug where `local-gateway create` ignored</span></span> `--local-address-prefixes`
* <span data-ttu-id="a0e85-2111">Ajout de la prise en charge de `--dns-servers` à</span><span class="sxs-lookup"><span data-stu-id="a0e85-2111">Added support for `--dns-servers` to</span></span> `vnet update`
* <span data-ttu-id="a0e85-2112">Correction d’un bogue lors de la création d’un appairage sans filtrage de route avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-2112">Fixed bug when creating a peering without route filtering with</span></span> `express-route peering create`
* <span data-ttu-id="a0e85-2113">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec</span><span class="sxs-lookup"><span data-stu-id="a0e85-2113">Fixed bug where `--provider` and `--bandwidth` arguments did not work with</span></span> `express-route update`
* <span data-ttu-id="a0e85-2114">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-2114">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a0e85-2115">Amélioration de la mise en forme de la sortie pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-2115">Improved output formatting for</span></span> `network list-usages`
* <span data-ttu-id="a0e85-2116">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a0e85-2116">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a0e85-2117">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a0e85-2117">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a0e85-2118">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a0e85-2118">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a0e85-2119">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="a0e85-2119">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a0e85-2120">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-2120">Profile</span></span>

* <span data-ttu-id="a0e85-2121">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="a0e85-2121">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a0e85-2122">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2122">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a0e85-2123">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="a0e85-2123">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a0e85-2124">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="a0e85-2124">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a0e85-2125">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="a0e85-2125">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a0e85-2126">SGBDR</span><span class="sxs-lookup"><span data-stu-id="a0e85-2126">RDBMS</span></span>

* <span data-ttu-id="a0e85-2127">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2127">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a0e85-2128">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2128">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a0e85-2129">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2129">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a0e85-2130">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2130">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-2131">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-2131">Resource</span></span>

* <span data-ttu-id="a0e85-2132">Amélioration des invites pour les paramètres manquants de</span><span class="sxs-lookup"><span data-stu-id="a0e85-2132">Improved prompts for missing parameters for</span></span> `group deployment create`
* <span data-ttu-id="a0e85-2133">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a0e85-2133">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a0e85-2134">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a0e85-2134">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a0e85-2135">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="a0e85-2135">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a0e85-2136">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2136">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a0e85-2137">Correction de l’analyse `--resource-type` permettant à la commande `lock` d’accepter `<resource-namespace>` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2137">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and</span></span> `<resource-type>`
* <span data-ttu-id="a0e85-2138">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2138">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a0e85-2139">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="a0e85-2139">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-2140">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2140">Role</span></span>

* <span data-ttu-id="a0e85-2141">Prise en charge de la sortie au format de fichier d’authentification du SDK pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-2141">Support output in SDK auth file format for</span></span> `create-for-rbac`
* <span data-ttu-id="a0e85-2142">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2142">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a0e85-2143">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="a0e85-2143">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a0e85-2144">Affichage des avertissements de dépréciation lors de l’utilisation de</span><span class="sxs-lookup"><span data-stu-id="a0e85-2144">Show deprecation warnings when using</span></span> `--expanded-view`
* <span data-ttu-id="a0e85-2145">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2145">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a0e85-2146">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0e85-2146">Service Fabric</span></span>
* <span data-ttu-id="a0e85-2147">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2147">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a0e85-2148">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2148">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a0e85-2149">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2149">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-2150">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-2150">SQL</span></span>

* <span data-ttu-id="a0e85-2151">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2151">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a0e85-2152">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2152">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a0e85-2153">Ajout des commandes `sql db list-editions` et</span><span class="sxs-lookup"><span data-stu-id="a0e85-2153">Added commands `sql db list-editions` and</span></span> `sql elastic-pool list-editions`

### <a name="storage"></a><span data-ttu-id="a0e85-2154">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-2154">Storage</span></span>

* <span data-ttu-id="a0e85-2155">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2155">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a0e85-2156">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="a0e85-2156">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a0e85-2157">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2157">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a0e85-2158">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2158">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a0e85-2159">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2159">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a0e85-2160">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2160">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-2161">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2161">VM</span></span>

* <span data-ttu-id="a0e85-2162">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-2162">Support configuring nsg</span></span>
* <span data-ttu-id="a0e85-2163">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="a0e85-2163">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a0e85-2164">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="a0e85-2164">Support managed service identities</span></span>
* <span data-ttu-id="a0e85-2165">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait</span><span class="sxs-lookup"><span data-stu-id="a0e85-2165">Fixed issue where `cmss create` with an existing load balancer required</span></span> `--backend-pool-name`
* <span data-ttu-id="a0e85-2166">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="a0e85-2166">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a0e85-2167">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-2167">May 10, 2017</span></span>

<span data-ttu-id="a0e85-2168">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a0e85-2168">Version 2.0.6</span></span>

* <span data-ttu-id="a0e85-2169">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a0e85-2169">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a0e85-2170">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2170">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a0e85-2171">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-2171">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a0e85-2172">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a0e85-2172">Include Cognitive Services module</span></span>
* <span data-ttu-id="a0e85-2173">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a0e85-2173">Include Service Fabric module</span></span>
* <span data-ttu-id="a0e85-2174">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2174">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a0e85-2175">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="a0e85-2175">Add support for CDN commands</span></span>
* <span data-ttu-id="a0e85-2176">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="a0e85-2176">Remove Container module</span></span>
* <span data-ttu-id="a0e85-2177">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2177">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a0e85-2178">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2178">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a0e85-2179">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-2179">Core</span></span>

* <span data-ttu-id="a0e85-2180">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="a0e85-2180">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a0e85-2181">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2181">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a0e85-2182">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2182">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a0e85-2183">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2183">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a0e85-2184">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2184">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a0e85-2185">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2185">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a0e85-2186">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2186">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a0e85-2187">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2187">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a0e85-2188">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2188">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a0e85-2189">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="a0e85-2189">core: Improved performance</span></span>
* <span data-ttu-id="a0e85-2190">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="a0e85-2190">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a0e85-2191">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="a0e85-2191">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-2192">ACS</span></span>

* <span data-ttu-id="a0e85-2193">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="a0e85-2193">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a0e85-2194">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="a0e85-2194">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a0e85-2195">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="a0e85-2195">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a0e85-2196">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2196">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-2197">AppService</span></span>

* <span data-ttu-id="a0e85-2198">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2198">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a0e85-2199">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="a0e85-2199">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a0e85-2200">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2200">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a0e85-2201">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="a0e85-2201">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a0e85-2202">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="a0e85-2202">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a0e85-2203">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2203">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a0e85-2204">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="a0e85-2204">support slot swap with preview</span></span>
* <span data-ttu-id="a0e85-2205">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2205">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a0e85-2206">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2206">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a0e85-2207">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-2207">CosmosDB</span></span>

* <span data-ttu-id="a0e85-2208">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a0e85-2208">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a0e85-2209">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="a0e85-2209">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a0e85-2210">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="a0e85-2210">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a0e85-2211">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="a0e85-2211">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a0e85-2212">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0e85-2212">Data Lake Analytics</span></span>

* <span data-ttu-id="a0e85-2213">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="a0e85-2213">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a0e85-2214">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2214">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a0e85-2215">accessible via :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2215">accessed through:</span></span> `az dla catalog package`
* <span data-ttu-id="a0e85-2216">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2216">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a0e85-2217">Table</span><span class="sxs-lookup"><span data-stu-id="a0e85-2217">Table</span></span>
  * <span data-ttu-id="a0e85-2218">Fonction table</span><span class="sxs-lookup"><span data-stu-id="a0e85-2218">Table valued function</span></span>
  * <span data-ttu-id="a0e85-2219">Affichage</span><span class="sxs-lookup"><span data-stu-id="a0e85-2219">View</span></span>
  * <span data-ttu-id="a0e85-2220">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2220">Table Statistics.</span></span> <span data-ttu-id="a0e85-2221">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="a0e85-2221">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a0e85-2222">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-2222">Data Lake Store</span></span>

* <span data-ttu-id="a0e85-2223">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="a0e85-2223">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a0e85-2224">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2224">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a0e85-2225">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2225">missed help for access show.</span></span> <span data-ttu-id="a0e85-2226">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2226">adding it.</span></span> <span data-ttu-id="a0e85-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a0e85-2228">Rechercher</span><span class="sxs-lookup"><span data-stu-id="a0e85-2228">Find</span></span>

* <span data-ttu-id="a0e85-2229">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="a0e85-2229">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a0e85-2230">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a0e85-2230">KeyVault</span></span>

* <span data-ttu-id="a0e85-2231">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="a0e85-2231">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a0e85-2232">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="a0e85-2232">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a0e85-2233">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="a0e85-2233">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a0e85-2234">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-2234">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a0e85-2235">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2235">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a0e85-2236">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2236">Lab</span></span>

* <span data-ttu-id="a0e85-2237">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2237">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a0e85-2238">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2238">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a0e85-2239">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2239">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a0e85-2240">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2240">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a0e85-2241">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="a0e85-2241">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a0e85-2242">Surveiller</span><span class="sxs-lookup"><span data-stu-id="a0e85-2242">Monitor</span></span>

* <span data-ttu-id="a0e85-2243">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2243">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a0e85-2244">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2244">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a0e85-2245">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-2245">Network</span></span>

* <span data-ttu-id="a0e85-2246">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2246">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a0e85-2247">Ajout de la prise en charge du paramètre `--filters` pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-2247">Add support for `--filters` parameter for</span></span> `network watcher packet-capture create`
* <span data-ttu-id="a0e85-2248">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a0e85-2248">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a0e85-2249">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="a0e85-2249">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a0e85-2250">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="a0e85-2250">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a0e85-2251">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a0e85-2251">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a0e85-2252">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a0e85-2252">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a0e85-2253">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="a0e85-2253">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a0e85-2254">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2254">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a0e85-2255">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="a0e85-2255">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a0e85-2256">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="a0e85-2256">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a0e85-2257">BC : correction d’un bogue dans la sortie de</span><span class="sxs-lookup"><span data-stu-id="a0e85-2257">BC: Fix bug in the output of</span></span> `vpn-connection create`
* <span data-ttu-id="a0e85-2258">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-2258">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a0e85-2259">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="a0e85-2259">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a0e85-2260">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="a0e85-2260">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a0e85-2261">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="a0e85-2261">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a0e85-2262">Profil</span><span class="sxs-lookup"><span data-stu-id="a0e85-2262">Profile</span></span>

* <span data-ttu-id="a0e85-2263">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2263">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a0e85-2264">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2264">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a0e85-2265">Redis</span><span class="sxs-lookup"><span data-stu-id="a0e85-2265">Redis</span></span>

* <span data-ttu-id="a0e85-2266">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="a0e85-2266">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a0e85-2267">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="a0e85-2267">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a0e85-2268">Ressource</span><span class="sxs-lookup"><span data-stu-id="a0e85-2268">Resource</span></span>

* <span data-ttu-id="a0e85-2269">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2269">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a0e85-2270">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2270">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a0e85-2271">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2271">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a0e85-2272">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2272">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a0e85-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a0e85-2274">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2274">Add docs for az lock update.</span></span> <span data-ttu-id="a0e85-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a0e85-2276">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2276">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a0e85-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a0e85-2278">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2278">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a0e85-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a0e85-2280">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2280">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a0e85-2281">Rôle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2281">Role</span></span>

* <span data-ttu-id="a0e85-2282">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2282">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a0e85-2283">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2283">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a0e85-2284">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2284">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a0e85-2285">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="a0e85-2285">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a0e85-2286">SQL</span><span class="sxs-lookup"><span data-stu-id="a0e85-2286">SQL</span></span>

* <span data-ttu-id="a0e85-2287">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="a0e85-2287">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a0e85-2288">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2288">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a0e85-2289">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-2289">Storage</span></span>

* <span data-ttu-id="a0e85-2290">Emplacement par défaut défini sur l’emplacement du groupe de ressources pour</span><span class="sxs-lookup"><span data-stu-id="a0e85-2290">Default location to resource group location for</span></span> `storage account create`
* <span data-ttu-id="a0e85-2291">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="a0e85-2291">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a0e85-2292">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="a0e85-2292">Add support for large block blob upload</span></span>
* <span data-ttu-id="a0e85-2293">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="a0e85-2293">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-2294">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2294">VM</span></span>

* <span data-ttu-id="a0e85-2295">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="a0e85-2295">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a0e85-2296">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2296">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a0e85-2297">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a0e85-2297">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a0e85-2298">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a0e85-2298">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a0e85-2299">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="a0e85-2299">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a0e85-2300">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="a0e85-2300">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a0e85-2301">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2301">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a0e85-2302">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-2302">April 3, 2017</span></span>

<span data-ttu-id="a0e85-2303">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a0e85-2303">Version 2.0.2</span></span>

<span data-ttu-id="a0e85-2304">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="a0e85-2304">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a0e85-2305">Principal</span><span class="sxs-lookup"><span data-stu-id="a0e85-2305">Core</span></span>

* <span data-ttu-id="a0e85-2306">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-2306">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a0e85-2307">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2307">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a0e85-2308">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2308">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a0e85-2309">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2309">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a0e85-2310">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2310">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a0e85-2311">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2311">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a0e85-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a0e85-2313">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="a0e85-2313">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a0e85-2314">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="a0e85-2314">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a0e85-2315">ACS</span><span class="sxs-lookup"><span data-stu-id="a0e85-2315">ACS</span></span>

* <span data-ttu-id="a0e85-2316">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2316">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a0e85-2317">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2317">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a0e85-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a0e85-2319">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2319">Add support for windows clusters.</span></span> <span data-ttu-id="a0e85-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a0e85-2321">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2321">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a0e85-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a0e85-2323">AppService</span><span class="sxs-lookup"><span data-stu-id="a0e85-2323">AppService</span></span>

* <span data-ttu-id="a0e85-2324">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2324">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a0e85-2325">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2325">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a0e85-2326">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2326">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a0e85-2327">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2327">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a0e85-2328">DataLake</span><span class="sxs-lookup"><span data-stu-id="a0e85-2328">DataLake</span></span>

* <span data-ttu-id="a0e85-2329">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a0e85-2329">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a0e85-2330">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a0e85-2330">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a0e85-2331">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a0e85-2331">DocuemntDB</span></span>

* <span data-ttu-id="a0e85-2332">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2332">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a0e85-2333">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="a0e85-2333">VM</span></span>

* <span data-ttu-id="a0e85-2334">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2334">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a0e85-2335">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2335">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a0e85-2336">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2336">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a0e85-2337">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2337">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a0e85-2338">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2338">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a0e85-2339">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2339">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="a0e85-2340">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a0e85-2340">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a0e85-2341">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="a0e85-2341">February 27, 2017</span></span>

<span data-ttu-id="a0e85-2342">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a0e85-2342">Version 2.0.0</span></span>

<span data-ttu-id="a0e85-2343">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2343">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a0e85-2344">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2344">Container Service (acs)</span></span>
- <span data-ttu-id="a0e85-2345">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2345">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a0e85-2346">Réseau</span><span class="sxs-lookup"><span data-stu-id="a0e85-2346">Networking</span></span>
- <span data-ttu-id="a0e85-2347">Stockage</span><span class="sxs-lookup"><span data-stu-id="a0e85-2347">Storage</span></span>

<span data-ttu-id="a0e85-2348">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2348">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a0e85-2349">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2349">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a0e85-2350">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2350">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a0e85-2351">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2351">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a0e85-2352">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a0e85-2352">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a0e85-2353">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="a0e85-2353">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a0e85-2354">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="a0e85-2354">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a0e85-2355">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a0e85-2355">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a0e85-2356">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a0e85-2356">Provide feedback from the command line with the `az feedback` command</span></span>

