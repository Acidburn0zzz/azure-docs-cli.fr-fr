---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8307ca9797a9a780d7e08d6d21cb66446c7e289
ms.sourcegitcommit: 6d9e8ee6dd07cfd07239a2948304d7f50ef781cc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2019
ms.locfileid: "58508900"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="c4ecf-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-103">Azure CLI release notes</span></span>
## <a name="march-26-2019"></a><span data-ttu-id="c4ecf-104">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-104">March 26, 2019</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-105">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-105">Core</span></span>
* <span data-ttu-id="c4ecf-106">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-106">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="c4ecf-107">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-107">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="c4ecf-108">Cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-108">Cloud</span></span>
* <span data-ttu-id="c4ecf-109">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-109">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-110">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-110">ACR</span></span>
* <span data-ttu-id="c4ecf-111">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c4ecf-111">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="c4ecf-112">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-112">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="c4ecf-113">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="c4ecf-113">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="c4ecf-114">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-114">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-115">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-115">AppService</span></span>
* <span data-ttu-id="c4ecf-116">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-116">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="c4ecf-117">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-117">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="c4ecf-118">Service BOT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-118">BOT Service</span></span>
* <span data-ttu-id="c4ecf-119">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-119">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="c4ecf-120">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="c4ecf-120">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="c4ecf-121">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-121">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="c4ecf-122">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c4ecf-122">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-123">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-123">CDN</span></span>
* <span data-ttu-id="c4ecf-124">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-124">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="c4ecf-125">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-125">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="c4ecf-126">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="c4ecf-126">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c4ecf-127">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-127">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-128">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c4ecf-128">Cosmosdb</span></span>
* <span data-ttu-id="c4ecf-129">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="c4ecf-129">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="c4ecf-130">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-130">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-131">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-131">Interactive</span></span>
* <span data-ttu-id="c4ecf-132">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="c4ecf-132">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-133">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-133">Monitor</span></span>
* <span data-ttu-id="c4ecf-134">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-134">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-135">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-135">Network</span></span>
* <span data-ttu-id="c4ecf-136">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-136">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-137">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-137">Profile</span></span>
* <span data-ttu-id="c4ecf-138">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-138">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="c4ecf-139">Postgres</span><span class="sxs-lookup"><span data-stu-id="c4ecf-139">Postgres</span></span> 
* <span data-ttu-id="c4ecf-140">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="c4ecf-140">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="c4ecf-141">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-141">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-142">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-142">Resource</span></span>
* <span data-ttu-id="c4ecf-143">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-143">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="c4ecf-144">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-144">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="c4ecf-145">Graph</span><span class="sxs-lookup"><span data-stu-id="c4ecf-145">Graph</span></span>
* <span data-ttu-id="c4ecf-146">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-146">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="c4ecf-147">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-147">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="c4ecf-148">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-148">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="c4ecf-149">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-149">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="c4ecf-150">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="c4ecf-150">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-151">storage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-151">storage</span></span>
* <span data-ttu-id="c4ecf-152">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-152">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="c4ecf-153">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="c4ecf-153">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="c4ecf-154">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-154">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="c4ecf-155">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-155">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-156">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-156">VM</span></span>
* <span data-ttu-id="c4ecf-157">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-157">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="c4ecf-158">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-158">March 12, 2019</span></span>

<span data-ttu-id="c4ecf-159">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="c4ecf-159">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-160">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-160">Core</span></span>

* <span data-ttu-id="c4ecf-161">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="c4ecf-161">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-162">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-162">ACR</span></span>

* <span data-ttu-id="c4ecf-163">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="c4ecf-163">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-164">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-164">ACS</span></span>

* <span data-ttu-id="c4ecf-165">Modification permettant d’ignorer l’argument `--listen-address` de `aks browse` si `kubectl` ne le prend pas en charge</span><span class="sxs-lookup"><span data-stu-id="c4ecf-165">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-166">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-166">AppService</span></span>

* <span data-ttu-id="c4ecf-167">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="c4ecf-167">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="c4ecf-168">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-168">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="c4ecf-169">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-169">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="c4ecf-170">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-170">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="c4ecf-171">Botservice</span><span class="sxs-lookup"><span data-stu-id="c4ecf-171">Botservice</span></span>

* <span data-ttu-id="c4ecf-172">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c4ecf-172">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c4ecf-173">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="c4ecf-173">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="c4ecf-174">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-174">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="c4ecf-175">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="c4ecf-175">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-176">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-176">Container</span></span>

* <span data-ttu-id="c4ecf-177">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-177">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="c4ecf-178">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c4ecf-178">EventHub</span></span>

* <span data-ttu-id="c4ecf-179">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="c4ecf-179">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="c4ecf-180">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c4ecf-180">Find</span></span>

* <span data-ttu-id="c4ecf-181">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c4ecf-181">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c4ecf-182">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c4ecf-182">HDInsight</span></span>

* <span data-ttu-id="c4ecf-183">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-183">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-184">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-184">Network</span></span>

* <span data-ttu-id="c4ecf-185">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="c4ecf-185">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-186">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c4ecf-186">Rdbms</span></span>

* <span data-ttu-id="c4ecf-187">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="c4ecf-187">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-188">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-188">Role</span></span>

* <span data-ttu-id="c4ecf-189">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-189">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="c4ecf-190">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="c4ecf-190">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4ecf-191">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4ecf-191">Service Fabric</span></span>

* <span data-ttu-id="c4ecf-192">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="c4ecf-192">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="c4ecf-193">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-193">February 26, 2019</span></span>

<span data-ttu-id="c4ecf-194">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="c4ecf-194">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-195">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-195">Core</span></span>

* <span data-ttu-id="c4ecf-196">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-196">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-197">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-197">ACR</span></span>

* <span data-ttu-id="c4ecf-198">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-198">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="c4ecf-199">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="c4ecf-199">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-200">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-200">ACS</span></span>

* <span data-ttu-id="c4ecf-201">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-201">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-202">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-202">AppService</span></span>

* <span data-ttu-id="c4ecf-203">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-203">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-204">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-204">Batch</span></span>
* <span data-ttu-id="c4ecf-205">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-205">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="c4ecf-206">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-206">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="c4ecf-207">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="c4ecf-207">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="c4ecf-208">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-208">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="c4ecf-209">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="c4ecf-209">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="c4ecf-210">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-210">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-211">CosmosDB</span></span>

* <span data-ttu-id="c4ecf-212">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-212">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="c4ecf-213">Kusto</span><span class="sxs-lookup"><span data-stu-id="c4ecf-213">Kusto</span></span>

* <span data-ttu-id="c4ecf-214">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="c4ecf-214">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-215">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-215">Network</span></span>

* <span data-ttu-id="c4ecf-216">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-216">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="c4ecf-217">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-217">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="c4ecf-218">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-218">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="c4ecf-219">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-219">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="c4ecf-220">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-220">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="c4ecf-221">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-221">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="c4ecf-222">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-222">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-223">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-223">Resource</span></span>

* <span data-ttu-id="c4ecf-224">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-224">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="c4ecf-225">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-225">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="c4ecf-226">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-226">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="c4ecf-227">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-227">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="c4ecf-228">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-228">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-229">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-229">Role</span></span>

* <span data-ttu-id="c4ecf-230">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-230">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-231">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-231">VM</span></span>

* <span data-ttu-id="c4ecf-232">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-232">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="c4ecf-233">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-233">February 12, 2019</span></span>

<span data-ttu-id="c4ecf-234">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="c4ecf-234">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-235">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-235">Core</span></span>

* <span data-ttu-id="c4ecf-236">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="c4ecf-236">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="c4ecf-237">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="c4ecf-237">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-238">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-238">ACR</span></span>
* <span data-ttu-id="c4ecf-239">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-239">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="c4ecf-240">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-240">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-241">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-241">ACS</span></span>
* <span data-ttu-id="c4ecf-242">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-242">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="c4ecf-243">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-243">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="c4ecf-244">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-244">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="c4ecf-245">AMS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-245">AMS</span></span>
* <span data-ttu-id="c4ecf-246">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-246">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="c4ecf-247">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-247">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-248">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-248">Appservice</span></span>
* <span data-ttu-id="c4ecf-249">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-249">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="c4ecf-250">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="c4ecf-250">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="c4ecf-251">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-251">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="c4ecf-252">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="c4ecf-252">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="c4ecf-253">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="c4ecf-253">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="c4ecf-254">Botservice</span><span class="sxs-lookup"><span data-stu-id="c4ecf-254">Botservice</span></span>
* <span data-ttu-id="c4ecf-255">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-255">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="c4ecf-256">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-256">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="c4ecf-257">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-257">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="c4ecf-258">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="c4ecf-258">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="c4ecf-259">[DÉPRÉCIÉ] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-259">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="c4ecf-260">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="c4ecf-260">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="c4ecf-261">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-261">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="c4ecf-262">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="c4ecf-262">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="c4ecf-263">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-263">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="c4ecf-264">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="c4ecf-264">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="c4ecf-265">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-265">Key Vault</span></span>
* <span data-ttu-id="c4ecf-266">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-266">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-267">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-267">Monitor</span></span>
* <span data-ttu-id="c4ecf-268">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-268">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-269">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-269">Network</span></span>
* <span data-ttu-id="c4ecf-270">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="c4ecf-270">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="c4ecf-271">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c4ecf-271">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="c4ecf-272">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-272">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="c4ecf-273">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-273">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c4ecf-274">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c4ecf-274">Policy Insights</span></span>
* <span data-ttu-id="c4ecf-275">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="c4ecf-275">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-276">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-276">RDBMS</span></span>
* <span data-ttu-id="c4ecf-277">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-277">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="c4ecf-278">Redis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-278">Redis</span></span>
* <span data-ttu-id="c4ecf-279">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-279">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="c4ecf-280">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-280">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="c4ecf-281">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-281">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="c4ecf-282">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="c4ecf-282">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="c4ecf-283">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-283">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="c4ecf-284">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-284">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="c4ecf-285">[DÉPRÉCIÉ] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-285">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-286">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-286">Role</span></span>
* <span data-ttu-id="c4ecf-287">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-287">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="c4ecf-288">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-288">SQL VM</span></span>
* <span data-ttu-id="c4ecf-289">[DÉPRÉCIÉ] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-289">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-290">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-290">VM</span></span>
* <span data-ttu-id="c4ecf-291">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-291">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="c4ecf-292">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-292">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="c4ecf-293">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="c4ecf-293">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="c4ecf-294">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-294">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="c4ecf-295">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-295">January 31, 2019</span></span>

<span data-ttu-id="c4ecf-296">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="c4ecf-296">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-297">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-297">Core</span></span>

* <span data-ttu-id="c4ecf-298">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="c4ecf-298">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="c4ecf-299">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-299">January 28, 2019</span></span>

<span data-ttu-id="c4ecf-300">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="c4ecf-300">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-301">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-301">ACR</span></span>
* <span data-ttu-id="c4ecf-302">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="c4ecf-302">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-303">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-303">ACS</span></span>
* <span data-ttu-id="c4ecf-304">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c4ecf-304">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c4ecf-305">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-305">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="c4ecf-306">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-306">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="c4ecf-307">AMS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-307">AMS</span></span>
* <span data-ttu-id="c4ecf-308">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-308">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="c4ecf-309">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-309">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-310">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-310">Appservice</span></span>
* <span data-ttu-id="c4ecf-311">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-311">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="c4ecf-312">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="c4ecf-312">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="c4ecf-313">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="c4ecf-313">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-314">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-314">Container</span></span>
* <span data-ttu-id="c4ecf-315">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-315">Added `container start` command</span></span>
* <span data-ttu-id="c4ecf-316">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-316">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c4ecf-317">EventGrid</span><span class="sxs-lookup"><span data-stu-id="c4ecf-317">EventGrid</span></span>
* <span data-ttu-id="c4ecf-318">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-318">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="c4ecf-319">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-319">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="c4ecf-320">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="c4ecf-320">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="c4ecf-321">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-321">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="c4ecf-322">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-322">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c4ecf-323">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c4ecf-323">HDInsight</span></span>
* <span data-ttu-id="c4ecf-324">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-324">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="c4ecf-325">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c4ecf-325">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="c4ecf-326">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-326">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="c4ecf-327">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-327">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="c4ecf-328">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-328">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="c4ecf-329">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-329">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-330">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-330">IoT</span></span>
* <span data-ttu-id="c4ecf-331">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="c4ecf-331">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="c4ecf-332">Kusto</span><span class="sxs-lookup"><span data-stu-id="c4ecf-332">Kusto</span></span>
* <span data-ttu-id="c4ecf-333">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-333">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-334">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-334">Monitor</span></span>
* <span data-ttu-id="c4ecf-335">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-335">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-336">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-336">Profile</span></span>
* <span data-ttu-id="c4ecf-337">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-337">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-338">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-338">Network</span></span>
* <span data-ttu-id="c4ecf-339">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="c4ecf-339">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="c4ecf-340">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="c4ecf-340">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-341">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-341">Resource</span></span>
* <span data-ttu-id="c4ecf-342">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-342">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="c4ecf-343">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-343">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="c4ecf-344">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-344">SQL Virtual Machine</span></span>
* <span data-ttu-id="c4ecf-345">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-345">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-346">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-346">Storage</span></span>
* <span data-ttu-id="c4ecf-347">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="c4ecf-347">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="c4ecf-348">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-348">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-349">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-349">VM</span></span>
* <span data-ttu-id="c4ecf-350">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-350">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="c4ecf-351">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-351">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="c4ecf-352">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="c4ecf-352">January 15, 2019</span></span>

<span data-ttu-id="c4ecf-353">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="c4ecf-353">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-354">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-354">ACR</span></span>
* <span data-ttu-id="c4ecf-355">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-355">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="c4ecf-356">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c4ecf-356">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="c4ecf-357">[DÉPRÉCIÉ] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-357">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="c4ecf-358">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-358">ACS</span></span>
* <span data-ttu-id="c4ecf-359">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-359">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-360">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-360">Appservice</span></span>
* <span data-ttu-id="c4ecf-361">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="c4ecf-361">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="c4ecf-362">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-362">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="c4ecf-363">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-363">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="c4ecf-364">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-364">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="c4ecf-365">Botservice</span><span class="sxs-lookup"><span data-stu-id="c4ecf-365">Botservice</span></span>
* <span data-ttu-id="c4ecf-366">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-366">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="c4ecf-367">Configuration</span><span class="sxs-lookup"><span data-stu-id="c4ecf-367">Configure</span></span>
* <span data-ttu-id="c4ecf-368">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="c4ecf-368">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-369">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-369">CosmosDB</span></span>
* <span data-ttu-id="c4ecf-370">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-370">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c4ecf-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c4ecf-371">HDInsight</span></span>
* <span data-ttu-id="c4ecf-372">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="c4ecf-372">Added commands for managing applications</span></span>
* <span data-ttu-id="c4ecf-373">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="c4ecf-373">Added commands for managing script actions</span></span>
* <span data-ttu-id="c4ecf-374">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-374">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="c4ecf-375">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-375">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="c4ecf-376">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-376">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-377">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-377">Network</span></span>
* <span data-ttu-id="c4ecf-378">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-378">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="c4ecf-379">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="c4ecf-379">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="c4ecf-380">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-380">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="c4ecf-381">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-381">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-382">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-382">Role</span></span>
* <span data-ttu-id="c4ecf-383">[DÉPRÉCIÉ] Dépréciation de l’argument `--password` au profit de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-383">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="c4ecf-384">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="c4ecf-384">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="c4ecf-385">Sécurité</span><span class="sxs-lookup"><span data-stu-id="c4ecf-385">Security</span></span>
* <span data-ttu-id="c4ecf-386">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-386">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-387">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-387">Storage</span></span>
* <span data-ttu-id="c4ecf-388">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-388">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="c4ecf-389">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="c4ecf-389">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="c4ecf-390">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-390">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="c4ecf-391">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-391">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="c4ecf-392">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-392">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-393">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-393">VM</span></span>
* <span data-ttu-id="c4ecf-394">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="c4ecf-394">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="c4ecf-395">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-395">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4ecf-396">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-396">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="c4ecf-397">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-397">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="c4ecf-398">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-398">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="c4ecf-399">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="c4ecf-399">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="c4ecf-400">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-400">December 20, 2018</span></span>

<span data-ttu-id="c4ecf-401">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="c4ecf-401">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="c4ecf-402">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-402">Appservice</span></span>
* <span data-ttu-id="c4ecf-403">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-403">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="c4ecf-404">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="c4ecf-404">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="c4ecf-405">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-405">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c4ecf-406">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c4ecf-406">IoTCentral</span></span>
* <span data-ttu-id="c4ecf-407">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="c4ecf-407">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-408">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-408">Role</span></span>
* <span data-ttu-id="c4ecf-409">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-409">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-410">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-410">SQL</span></span>
* <span data-ttu-id="c4ecf-411">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-411">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-412">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-412">VM</span></span>
* <span data-ttu-id="c4ecf-413">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-413">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="c4ecf-414">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-414">December 18, 2018</span></span>

<span data-ttu-id="c4ecf-415">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="c4ecf-415">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="c4ecf-416">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-416">ACR</span></span>
* <span data-ttu-id="c4ecf-417">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-417">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="c4ecf-418">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="c4ecf-418">Condensed the table layout for task list</span></span>
* <span data-ttu-id="c4ecf-419">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="c4ecf-419">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-420">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-420">ACS</span></span>
* <span data-ttu-id="c4ecf-421">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="c4ecf-421">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="c4ecf-422">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-422">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="c4ecf-423">[DÉCONSEILLÉ] Commandes `az acs` déconseillées.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-423">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="c4ecf-424">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-424">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="c4ecf-425">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-425">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="c4ecf-426">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="c4ecf-426">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-427">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-427">Appservice</span></span>
* <span data-ttu-id="c4ecf-428">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-428">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="c4ecf-429">Botservice</span><span class="sxs-lookup"><span data-stu-id="c4ecf-429">Botservice</span></span>
* <span data-ttu-id="c4ecf-430">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-430">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="c4ecf-431">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="c4ecf-431">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="c4ecf-432">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="c4ecf-432">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="c4ecf-433">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-433">Reduced Kudu network calls</span></span>
* <span data-ttu-id="c4ecf-434">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="c4ecf-434">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-435">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-435">Consumption</span></span>
* <span data-ttu-id="c4ecf-436">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="c4ecf-436">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-437">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-437">CosmosDB</span></span>
* <span data-ttu-id="c4ecf-438">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-438">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="c4ecf-439">Cartes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-439">Maps</span></span>
* <span data-ttu-id="c4ecf-440">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-440">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-441">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-441">Network</span></span>
* <span data-ttu-id="c4ecf-442">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-442">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="c4ecf-443">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-443">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-444">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-444">Resource</span></span>
* <span data-ttu-id="c4ecf-445">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-445">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="c4ecf-446">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-446">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-447">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-447">Storage</span></span>
*  <span data-ttu-id="c4ecf-448">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-448">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-449">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-449">VM</span></span>
* <span data-ttu-id="c4ecf-450">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-450">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="c4ecf-451">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-451">December 4, 2018</span></span>

<span data-ttu-id="c4ecf-452">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="c4ecf-452">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="c4ecf-453">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-453">Core</span></span>
* <span data-ttu-id="c4ecf-454">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-454">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="c4ecf-455">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-455">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-456">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-456">Appservice</span></span>
* <span data-ttu-id="c4ecf-457">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-457">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="c4ecf-458">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-458">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-459">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-459">Network</span></span>
* <span data-ttu-id="c4ecf-460">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="c4ecf-460">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-461">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-461">Role</span></span>
* <span data-ttu-id="c4ecf-462">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-462">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="c4ecf-463">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-463">VM</span></span>
* <span data-ttu-id="c4ecf-464">[DÉCONSEILLÉ] Le paramètre `vm extension [show|wait] --expand` est déconseillé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-464">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="c4ecf-465">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-465">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="c4ecf-466">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-466">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="c4ecf-467">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-467">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="c4ecf-468">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-468">November 20, 2018</span></span>

<span data-ttu-id="c4ecf-469">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="c4ecf-469">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="c4ecf-470">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-470">Core</span></span>
* <span data-ttu-id="c4ecf-471">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="c4ecf-471">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-472">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-472">ACR</span></span>
* <span data-ttu-id="c4ecf-473">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="c4ecf-473">Added context token to task step</span></span>
* <span data-ttu-id="c4ecf-474">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="c4ecf-474">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="c4ecf-475">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-475">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-476">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-476">Appservice</span></span>
* <span data-ttu-id="c4ecf-477">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-477">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="c4ecf-478">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-478">Updated the default `node_version`.</span></span> <span data-ttu-id="c4ecf-479">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="c4ecf-479">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="c4ecf-480">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-480">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="c4ecf-481">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="c4ecf-481">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="c4ecf-482">IotCentral</span><span class="sxs-lookup"><span data-stu-id="c4ecf-482">IotCentral</span></span>
* <span data-ttu-id="c4ecf-483">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="c4ecf-483">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-484">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-484">KeyVault</span></span>
* <span data-ttu-id="c4ecf-485">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-485">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-486">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-486">Network</span></span>
* <span data-ttu-id="c4ecf-487">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="c4ecf-487">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="c4ecf-488">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-488">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="c4ecf-489">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-489">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="c4ecf-490">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-490">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-491">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c4ecf-491">Rdbms</span></span>
* <span data-ttu-id="c4ecf-492">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="c4ecf-492">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="c4ecf-493">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-493">Rbac</span></span>
* <span data-ttu-id="c4ecf-494">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-494">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="c4ecf-495">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-495">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="c4ecf-496">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-496">Storage</span></span>
* <span data-ttu-id="c4ecf-497">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-497">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="c4ecf-498">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-498">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="c4ecf-499">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-499">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="c4ecf-500">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-500">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-501">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-501">VM</span></span>
* <span data-ttu-id="c4ecf-502">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="c4ecf-502">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="c4ecf-503">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-503">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="c4ecf-504">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-504">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="c4ecf-505">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-505">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="c4ecf-506">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-506">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="c4ecf-507">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-507">Added `snapshot wait` command</span></span>
* <span data-ttu-id="c4ecf-508">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-508">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="c4ecf-509">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-509">November 6, 2018</span></span>

<span data-ttu-id="c4ecf-510">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="c4ecf-510">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-511">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-511">Core</span></span>
* <span data-ttu-id="c4ecf-512">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="c4ecf-512">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-513">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-513">ACR</span></span>
* <span data-ttu-id="c4ecf-514">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="c4ecf-514">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="c4ecf-515">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="c4ecf-515">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-516">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-516">ACS</span></span>
* <span data-ttu-id="c4ecf-517">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-517">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="c4ecf-518">Advisor</span><span class="sxs-lookup"><span data-stu-id="c4ecf-518">Advisor</span></span>
* <span data-ttu-id="c4ecf-519">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-519">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="c4ecf-520">AMS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-520">AMS</span></span>
* <span data-ttu-id="c4ecf-521">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-521">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="c4ecf-522">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-522">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="c4ecf-523">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-523">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="c4ecf-524">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="c4ecf-524">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="c4ecf-525">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-525">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="c4ecf-526">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-526">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="c4ecf-527">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-527">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="c4ecf-528">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-528">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="c4ecf-529">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-529">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="c4ecf-530">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-530">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="c4ecf-531">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-531">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="c4ecf-532">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-532">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="c4ecf-533">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="c4ecf-533">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="c4ecf-534">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-534">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="c4ecf-535">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-535">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="c4ecf-536">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="c4ecf-536">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="c4ecf-537">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-537">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-538">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-538">AppService</span></span>
* <span data-ttu-id="c4ecf-539">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-539">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="c4ecf-540">Configuration</span><span class="sxs-lookup"><span data-stu-id="c4ecf-540">Configure</span></span>
* <span data-ttu-id="c4ecf-541">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-541">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-542">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-542">Container</span></span>
* <span data-ttu-id="c4ecf-543">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="c4ecf-543">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="c4ecf-544">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c4ecf-544">EventHub</span></span>
* <span data-ttu-id="c4ecf-545">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-545">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-546">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-546">Interactive</span></span>
* <span data-ttu-id="c4ecf-547">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="c4ecf-547">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-548">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-548">Monitor</span></span>
* <span data-ttu-id="c4ecf-549">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-549">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-550">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-550">Network</span></span>
* <span data-ttu-id="c4ecf-551">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-551">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="c4ecf-552">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-552">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="c4ecf-553">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-553">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="c4ecf-554">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-554">Profile</span></span>
* <span data-ttu-id="c4ecf-555">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-555">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-556">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-556">RDBMS</span></span>
* <span data-ttu-id="c4ecf-557">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="c4ecf-557">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-558">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-558">Resource</span></span>
* <span data-ttu-id="c4ecf-559">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-559">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-560">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-560">Role</span></span>
* <span data-ttu-id="c4ecf-561">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="c4ecf-561">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="c4ecf-562">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-562">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="c4ecf-563">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="c4ecf-563">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-564">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-564">Storage</span></span>
* <span data-ttu-id="c4ecf-565">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-565">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-566">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-566">VM</span></span>
* <span data-ttu-id="c4ecf-567">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-567">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="c4ecf-568">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-568">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="c4ecf-569">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="c4ecf-569">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="c4ecf-570">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="c4ecf-570">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="c4ecf-571">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="c4ecf-571">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="c4ecf-572">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-572">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="c4ecf-573">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-573">October 23, 2018</span></span>

<span data-ttu-id="c4ecf-574">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="c4ecf-574">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-575">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-575">Core</span></span>
* <span data-ttu-id="c4ecf-576">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-576">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="c4ecf-577">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-577">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-578">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-578">ACR</span></span>
* <span data-ttu-id="c4ecf-579">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-579">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-580">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-580">CDN</span></span>
* <span data-ttu-id="c4ecf-581">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-581">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="c4ecf-582">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-582">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-583">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-583">Container</span></span>
* <span data-ttu-id="c4ecf-584">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="c4ecf-584">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="c4ecf-585">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-585">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="c4ecf-586">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="c4ecf-586">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="c4ecf-587">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-587">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="c4ecf-588">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c4ecf-588">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="c4ecf-589">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="c4ecf-589">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="c4ecf-590">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-590">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-591">CosmosDB</span></span>
* <span data-ttu-id="c4ecf-592">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-592">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-593">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-593">Interactive</span></span>
* <span data-ttu-id="c4ecf-594">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="c4ecf-594">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="c4ecf-595">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c4ecf-595">IoT Central</span></span>
* <span data-ttu-id="c4ecf-596">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="c4ecf-596">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="c4ecf-597">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="c4ecf-597">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-598">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-598">Monitor</span></span>
* <span data-ttu-id="c4ecf-599">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-599">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="c4ecf-600">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-600">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="c4ecf-601">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c4ecf-601">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c4ecf-602">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-602">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="c4ecf-603">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-603">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="c4ecf-604">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-604">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="c4ecf-605">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-605">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="c4ecf-606">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="c4ecf-606">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="c4ecf-607">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-607">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="c4ecf-608">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-608">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-609">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-609">Network</span></span>
* <span data-ttu-id="c4ecf-610">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-610">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="c4ecf-611">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-611">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="c4ecf-612">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-612">ServiceBus</span></span>
* <span data-ttu-id="c4ecf-613">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-613">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-614">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-614">SQL</span></span>
* <span data-ttu-id="c4ecf-615">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-615">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-616">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-616">Storage</span></span>
* <span data-ttu-id="c4ecf-617">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="c4ecf-617">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="c4ecf-618">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-618">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-619">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-619">VM</span></span>
* <span data-ttu-id="c4ecf-620">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-620">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4ecf-621">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-621">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="c4ecf-622">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-622">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="c4ecf-623">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-623">October 16, 2018</span></span>

<span data-ttu-id="c4ecf-624">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="c4ecf-624">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-625">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-625">VM</span></span>
* <span data-ttu-id="c4ecf-626">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="c4ecf-626">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="c4ecf-627">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-627">October 9, 2018</span></span>

<span data-ttu-id="c4ecf-628">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="c4ecf-628">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-629">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-629">Core</span></span>
* <span data-ttu-id="c4ecf-630">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-630">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-631">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-631">ACR</span></span>
* <span data-ttu-id="c4ecf-632">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="c4ecf-632">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-633">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-633">ACS</span></span>
* <span data-ttu-id="c4ecf-634">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="c4ecf-634">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="c4ecf-635">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="c4ecf-635">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="c4ecf-636">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-636">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="c4ecf-637">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-637">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-638">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-638">Container</span></span>
* <span data-ttu-id="c4ecf-639">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-639">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="c4ecf-640">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-640">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="c4ecf-641">Event Hub</span><span class="sxs-lookup"><span data-stu-id="c4ecf-641">Event Hub</span></span>
* <span data-ttu-id="c4ecf-642">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-642">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="c4ecf-643">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-643">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="c4ecf-644">Extensions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-644">Extensions</span></span>
* <span data-ttu-id="c4ecf-645">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-645">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="c4ecf-646">HDInsight</span><span class="sxs-lookup"><span data-stu-id="c4ecf-646">HDInsight</span></span>
* <span data-ttu-id="c4ecf-647">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-647">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-648">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-648">IoT</span></span>
* <span data-ttu-id="c4ecf-649">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="c4ecf-649">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-650">KeyVault</span></span>
* <span data-ttu-id="c4ecf-651">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="c4ecf-651">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-652">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-652">Network</span></span>
* <span data-ttu-id="c4ecf-653">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-653">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="c4ecf-654">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="c4ecf-654">See #6052</span></span>
* <span data-ttu-id="c4ecf-655">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-655">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="c4ecf-656">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="c4ecf-656">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="c4ecf-657">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-657">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="c4ecf-658">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-658">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="c4ecf-659">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-659">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="c4ecf-660">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-660">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-661">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-661">Role</span></span>
* <span data-ttu-id="c4ecf-662">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-662">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="c4ecf-663">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-663">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="c4ecf-664">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="c4ecf-664">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="c4ecf-665">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-665">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="c4ecf-666">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-666">Service Bus</span></span>
* <span data-ttu-id="c4ecf-667">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-667">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-668">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-668">VM</span></span>
* <span data-ttu-id="c4ecf-669">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-669">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="c4ecf-670">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-670">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="c4ecf-671">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-671">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="c4ecf-672">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-672">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="c4ecf-673">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-673">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="c4ecf-674">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-674">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="c4ecf-675">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-675">September 21, 2018</span></span>

<span data-ttu-id="c4ecf-676">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="c4ecf-676">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-677">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-677">ACR</span></span>
* <span data-ttu-id="c4ecf-678">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-678">Added ACR Task commands</span></span>
* <span data-ttu-id="c4ecf-679">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-679">Added quick run command</span></span>
* <span data-ttu-id="c4ecf-680">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-680">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="c4ecf-681">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-681">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="c4ecf-682">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-682">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="c4ecf-683">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="c4ecf-683">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-684">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-684">ACS</span></span>
* <span data-ttu-id="c4ecf-685">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-685">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="c4ecf-686">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="c4ecf-686">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-687">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-687">AppService</span></span>

* <span data-ttu-id="c4ecf-688">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-688">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="c4ecf-689">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="c4ecf-689">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="c4ecf-690">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="c4ecf-690">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="c4ecf-691">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-691">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-692">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-692">Batch</span></span>
* <span data-ttu-id="c4ecf-693">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="c4ecf-693">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="c4ecf-694">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-694">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="c4ecf-695">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-695">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="c4ecf-696">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-696">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4ecf-697">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-697">Batch AI</span></span> 
* <span data-ttu-id="c4ecf-698">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-698">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4ecf-699">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-699">Cognitive Services</span></span>
* <span data-ttu-id="c4ecf-700">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-700">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="c4ecf-701">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-701">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="c4ecf-702">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-702">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="c4ecf-703">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-703">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="c4ecf-704">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-704">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="c4ecf-705">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-705">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-706">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-706">Container</span></span>
* <span data-ttu-id="c4ecf-707">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="c4ecf-707">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="c4ecf-708">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-708">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="c4ecf-709">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-709">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="c4ecf-710">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-710">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="c4ecf-711">DataLake</span><span class="sxs-lookup"><span data-stu-id="c4ecf-711">Datalake</span></span>
* <span data-ttu-id="c4ecf-712">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-712">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="c4ecf-713">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-713">Interactive Shell</span></span>
* <span data-ttu-id="c4ecf-714">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-714">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="c4ecf-715">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-715">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-716">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-716">IoT</span></span>
* <span data-ttu-id="c4ecf-717">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-717">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="c4ecf-718">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-718">Key Vault</span></span>
* <span data-ttu-id="c4ecf-719">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="c4ecf-719">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-720">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-720">Network</span></span>
* <span data-ttu-id="c4ecf-721">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-721">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="c4ecf-722">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-722">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="c4ecf-723">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="c4ecf-723">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="c4ecf-724">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-724">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="c4ecf-725">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-725">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="c4ecf-726">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-726">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="c4ecf-727">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-727">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="c4ecf-728">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-728">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="c4ecf-729">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-729">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="c4ecf-730">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-730">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="c4ecf-731">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-731">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="c4ecf-732">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-732">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="c4ecf-733">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-733">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="c4ecf-734">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-734">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="c4ecf-735">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-735">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="c4ecf-736">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="c4ecf-736">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="c4ecf-737">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-737">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="c4ecf-738">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-738">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-739">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-739">RDBMS</span></span>
* <span data-ttu-id="c4ecf-740">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-740">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="c4ecf-741">Réservation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-741">Reservation</span></span>
* <span data-ttu-id="c4ecf-742">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-742">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="c4ecf-743">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-743">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="c4ecf-744">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="c4ecf-744">Manage App</span></span>
* <span data-ttu-id="c4ecf-745">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-745">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="c4ecf-746">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="c4ecf-746">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-747">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-747">Role</span></span>
* <span data-ttu-id="c4ecf-748">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-748">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="c4ecf-749">SignalR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-749">SignalR</span></span>
* <span data-ttu-id="c4ecf-750">Première version</span><span class="sxs-lookup"><span data-stu-id="c4ecf-750">First release</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-751">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-751">Storage</span></span>
* <span data-ttu-id="c4ecf-752">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="c4ecf-752">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="c4ecf-753">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="c4ecf-753">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-754">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-754">VM</span></span>
* <span data-ttu-id="c4ecf-755">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-755">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="c4ecf-756">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-756">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="c4ecf-757">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-757">August 28, 2018</span></span>

<span data-ttu-id="c4ecf-758">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="c4ecf-758">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-759">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-759">Core</span></span>

* <span data-ttu-id="c4ecf-760">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-760">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="c4ecf-761">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c4ecf-761">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-762">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-762">ACR</span></span>

* <span data-ttu-id="c4ecf-763">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="c4ecf-763">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="c4ecf-764">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-764">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-765">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-765">ACS</span></span>

* <span data-ttu-id="c4ecf-766">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-766">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="c4ecf-767">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="c4ecf-767">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-768">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-768">AppService</span></span>

* <span data-ttu-id="c4ecf-769">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="c4ecf-769">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="c4ecf-770">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="c4ecf-770">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="c4ecf-771">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-771">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="c4ecf-772">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c4ecf-772">Backup</span></span>

* <span data-ttu-id="c4ecf-773">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-773">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="c4ecf-774">Service de robot</span><span class="sxs-lookup"><span data-stu-id="c4ecf-774">Bot Service</span></span>

* <span data-ttu-id="c4ecf-775">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-775">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4ecf-776">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-776">Cognitive Services</span></span>

* <span data-ttu-id="c4ecf-777">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-777">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-778">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-778">IoT</span></span>

* <span data-ttu-id="c4ecf-779">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-779">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-780">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-780">Monitor</span></span>

* <span data-ttu-id="c4ecf-781">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-781">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="c4ecf-782">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-782">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-783">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-783">Network</span></span>

* <span data-ttu-id="c4ecf-784">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-784">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-785">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-785">Resource</span></span>

* <span data-ttu-id="c4ecf-786">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-786">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-787">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-787">Storage</span></span>

* <span data-ttu-id="c4ecf-788">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-788">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-789">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-789">VM</span></span>

* <span data-ttu-id="c4ecf-790">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-790">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="c4ecf-791">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-791">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="c4ecf-792">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-792">Auguest 14, 2018</span></span>

<span data-ttu-id="c4ecf-793">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="c4ecf-793">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-794">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-794">Core</span></span>

* <span data-ttu-id="c4ecf-795">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-795">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="c4ecf-796">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="c4ecf-796">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="c4ecf-797">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-797">Telemetry</span></span>

* <span data-ttu-id="c4ecf-798">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-798">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-799">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-799">ACR</span></span>

* <span data-ttu-id="c4ecf-800">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-800">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="c4ecf-801">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-801">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-802">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-802">ACS</span></span>

* <span data-ttu-id="c4ecf-803">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-803">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="c4ecf-804">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-804">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="c4ecf-805">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-805">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="c4ecf-806">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-806">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="c4ecf-807">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="c4ecf-807">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="c4ecf-808">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-808">AppService</span></span>

* <span data-ttu-id="c4ecf-809">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-809">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="c4ecf-810">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="c4ecf-810">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="c4ecf-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-811">BatchAI</span></span>

* <span data-ttu-id="c4ecf-812">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="c4ecf-812">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="c4ecf-813">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-813">Container</span></span>

* <span data-ttu-id="c4ecf-814">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-814">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="c4ecf-815">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-815">IoT</span></span>

* <span data-ttu-id="c4ecf-816">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="c4ecf-816">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="c4ecf-817">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-817">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="c4ecf-818">Iot Central</span><span class="sxs-lookup"><span data-stu-id="c4ecf-818">Iot Central</span></span>

* <span data-ttu-id="c4ecf-819">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="c4ecf-819">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-820">KeyVault</span></span>


* <span data-ttu-id="c4ecf-821">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-821">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="c4ecf-822">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-822">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="c4ecf-823">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="c4ecf-823">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="c4ecf-824">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-824">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="c4ecf-825">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-825">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="c4ecf-826">Relais</span><span class="sxs-lookup"><span data-stu-id="c4ecf-826">Relay</span></span>

* <span data-ttu-id="c4ecf-827">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-827">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-828">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-828">Sql</span></span>

* <span data-ttu-id="c4ecf-829">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-829">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-830">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-830">Storage</span></span>

* <span data-ttu-id="c4ecf-831">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="c4ecf-831">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="c4ecf-832">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-832">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="c4ecf-833">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-833">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="c4ecf-834">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="c4ecf-834">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="c4ecf-835">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-835">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-836">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-836">VM</span></span>

* <span data-ttu-id="c4ecf-837">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-837">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="c4ecf-838">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-838">July 31, 2018</span></span>

<span data-ttu-id="c4ecf-839">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="c4ecf-839">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-840">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-840">ACR</span></span>

* <span data-ttu-id="c4ecf-841">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-841">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="c4ecf-842">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-842">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-843">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-843">ACS</span></span>

* <span data-ttu-id="c4ecf-844">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-844">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-845">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-845">Batch</span></span>

* <span data-ttu-id="c4ecf-846">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c4ecf-846">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-847">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-847">Container</span></span>

* <span data-ttu-id="c4ecf-848">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="c4ecf-848">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-849">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-849">Network</span></span>

* <span data-ttu-id="c4ecf-850">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c4ecf-850">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="c4ecf-851">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-851">Resource</span></span>

* <span data-ttu-id="c4ecf-852">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-852">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="c4ecf-853">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-853">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-854">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-854">Role</span></span>

* <span data-ttu-id="c4ecf-855">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-855">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="c4ecf-856">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-856">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="c4ecf-857">Recherche</span><span class="sxs-lookup"><span data-stu-id="c4ecf-857">Search</span></span>

* <span data-ttu-id="c4ecf-858">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="c4ecf-858">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="c4ecf-859">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-859">Service Bus</span></span>

* <span data-ttu-id="c4ecf-860">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="c4ecf-860">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="c4ecf-861">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-861">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="c4ecf-862">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-862">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="c4ecf-863">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-864">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-864">Storage</span></span>

* <span data-ttu-id="c4ecf-865">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-865">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="c4ecf-866">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-866">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-867">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-867">VM</span></span>

* <span data-ttu-id="c4ecf-868">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-868">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="c4ecf-869">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-869">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="c4ecf-870">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="c4ecf-870">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="c4ecf-871">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-871">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="c4ecf-872">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-872">July 18, 2018</span></span>

<span data-ttu-id="c4ecf-873">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="c4ecf-873">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-874">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-874">Core</span></span>

* <span data-ttu-id="c4ecf-875">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-875">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="c4ecf-876">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-876">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="c4ecf-877">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-877">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-878">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-878">ACR</span></span>

* <span data-ttu-id="c4ecf-879">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-879">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="c4ecf-880">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-880">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="c4ecf-881">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-881">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="c4ecf-882">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-882">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-883">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-883">ACS</span></span>

* <span data-ttu-id="c4ecf-884">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="c4ecf-884">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-885">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-885">AppService</span></span>

* <span data-ttu-id="c4ecf-886">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-886">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-887">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-887">Batch</span></span>

* <span data-ttu-id="c4ecf-888">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c4ecf-888">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="c4ecf-889">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-889">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4ecf-890">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-890">Batch AI</span></span>

* <span data-ttu-id="c4ecf-891">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-891">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-892">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-892">Container</span></span>

* <span data-ttu-id="c4ecf-893">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="c4ecf-893">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="c4ecf-894">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="c4ecf-894">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-895">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-895">Network</span></span>

* <span data-ttu-id="c4ecf-896">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-896">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="c4ecf-897">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-897">Added `network nic wait`</span></span>
* <span data-ttu-id="c4ecf-898">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-898">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="c4ecf-899">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-899">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="c4ecf-900">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-900">Resource</span></span>

* <span data-ttu-id="c4ecf-901">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-901">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="c4ecf-902">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-902">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="c4ecf-903">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-903">Added `deployment wait` command</span></span>
* <span data-ttu-id="c4ecf-904">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="c4ecf-904">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-905">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-905">SQL</span></span>

* <span data-ttu-id="c4ecf-906">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-906">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="c4ecf-907">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-907">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="c4ecf-908">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-908">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-909">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-909">Storage</span></span>

* <span data-ttu-id="c4ecf-910">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="c4ecf-910">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-911">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-911">VM</span></span>

* <span data-ttu-id="c4ecf-912">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-912">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="c4ecf-913">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-913">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="c4ecf-914">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-914">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c4ecf-915">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-915">July 3, 2018</span></span>

<span data-ttu-id="c4ecf-916">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="c4ecf-916">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="c4ecf-917">AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-917">AKS</span></span>

* <span data-ttu-id="c4ecf-918">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-918">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c4ecf-919">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-919">July 3, 2018</span></span>

<span data-ttu-id="c4ecf-920">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="c4ecf-920">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-921">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-921">Core</span></span>

* <span data-ttu-id="c4ecf-922">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-922">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-923">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-923">ACR</span></span>

* <span data-ttu-id="c4ecf-924">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="c4ecf-924">Added polling build status</span></span>
* <span data-ttu-id="c4ecf-925">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-925">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="c4ecf-926">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-926">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-927">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-927">ACS</span></span>

* <span data-ttu-id="c4ecf-928">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-928">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="c4ecf-929">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-929">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="c4ecf-930">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-930">Updated options for `aks browse` command.</span></span> <span data-ttu-id="c4ecf-931">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-931">Added `--listen-port` support</span></span>
* <span data-ttu-id="c4ecf-932">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-932">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="c4ecf-933">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="c4ecf-933">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="c4ecf-934">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-934">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-935">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-935">AppService</span></span>

* <span data-ttu-id="c4ecf-936">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-936">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="c4ecf-937">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="c4ecf-937">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="c4ecf-938">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c4ecf-938">Backup</span></span>

* <span data-ttu-id="c4ecf-939">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="c4ecf-939">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="c4ecf-940">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-940">BatchAI</span></span>

* <span data-ttu-id="c4ecf-941">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-941">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="c4ecf-942">Cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-942">Cloud</span></span>

* <span data-ttu-id="c4ecf-943">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-943">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-944">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-944">Container</span></span>

* <span data-ttu-id="c4ecf-945">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="c4ecf-945">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="c4ecf-946">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-946">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="c4ecf-947">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="c4ecf-947">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-948">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-948">Extension</span></span>

* <span data-ttu-id="c4ecf-949">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-949">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-950">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-950">Network</span></span>

* <span data-ttu-id="c4ecf-951">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-951">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-952">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c4ecf-952">Rdbms</span></span>

* <span data-ttu-id="c4ecf-953">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-953">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-954">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-954">Resource</span></span>

* <span data-ttu-id="c4ecf-955">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-955">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-956">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-956">VM</span></span>

* <span data-ttu-id="c4ecf-957">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="c4ecf-957">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="c4ecf-958">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-958">June 25, 2018</span></span>

<span data-ttu-id="c4ecf-959">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="c4ecf-959">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="c4ecf-960">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-960">CLI</span></span>

* <span data-ttu-id="c4ecf-961">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-961">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="c4ecf-962">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-962">June 19, 2018</span></span>

<span data-ttu-id="c4ecf-963">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="c4ecf-963">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-964">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-964">Core</span></span>

* <span data-ttu-id="c4ecf-965">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-965">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-966">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-966">ACR</span></span>

* <span data-ttu-id="c4ecf-967">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="c4ecf-967">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="c4ecf-968">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-968">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-969">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-969">ACS</span></span>

* <span data-ttu-id="c4ecf-970">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-970">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="c4ecf-971">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-971">Added `--update` support</span></span>
* <span data-ttu-id="c4ecf-972">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-972">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="c4ecf-973">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-973">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="c4ecf-974">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-974">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="c4ecf-975">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-975">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="c4ecf-976">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-976">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="c4ecf-977">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-977">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-978">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-978">AppService</span></span>

* <span data-ttu-id="c4ecf-979">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-979">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="c4ecf-980">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-980">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-981">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-981">Batch</span></span>

* <span data-ttu-id="c4ecf-982">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-982">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4ecf-983">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-983">Batch AI</span></span>

* <span data-ttu-id="c4ecf-984">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-984">Added support for workspaces.</span></span> <span data-ttu-id="c4ecf-985">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-985">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="c4ecf-986">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-986">Added support for experiments.</span></span> <span data-ttu-id="c4ecf-987">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-987">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="c4ecf-988">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="c4ecf-988">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="c4ecf-989">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-989">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="c4ecf-990">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-990">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="c4ecf-991">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-991">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="c4ecf-992">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-992">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="c4ecf-993">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="c4ecf-993">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="c4ecf-994">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-994">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="c4ecf-995">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-995">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="c4ecf-996">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-996">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="c4ecf-997">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-997">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="c4ecf-998">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-998">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="c4ecf-999">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-999">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="c4ecf-1000">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1000">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="c4ecf-1001">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1001">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="c4ecf-1002">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1002">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="c4ecf-1003">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1003">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c4ecf-1004">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1004">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="c4ecf-1005">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1005">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="c4ecf-1006">Cartes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1006">Maps</span></span>

* <span data-ttu-id="c4ecf-1007">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1007">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1008">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1008">Network</span></span>

* <span data-ttu-id="c4ecf-1009">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1009">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="c4ecf-1010">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1010">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="c4ecf-1011">#6502</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1011">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="c4ecf-1012">Réservations</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1012">Reservations</span></span>

* <span data-ttu-id="c4ecf-1013">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1013">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="c4ecf-1014">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1014">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="c4ecf-1015">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1015">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="c4ecf-1016">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1016">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="c4ecf-1017">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1017">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="c4ecf-1018">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1018">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1019">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1019">Role</span></span>

* <span data-ttu-id="c4ecf-1020">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1020">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1021">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1021">SQL</span></span>

* <span data-ttu-id="c4ecf-1022">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1022">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1023">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1023">Storage</span></span>

* <span data-ttu-id="c4ecf-1024">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1024">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1025">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1025">VM</span></span>

* <span data-ttu-id="c4ecf-1026">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1026">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="c4ecf-1027">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1027">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="c4ecf-1028">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1028">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c4ecf-1029">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1029">June 13, 2018</span></span>

<span data-ttu-id="c4ecf-1030">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1030">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1031">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1031">Core</span></span>

* <span data-ttu-id="c4ecf-1032">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1032">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c4ecf-1033">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1033">June 13, 2018</span></span>

<span data-ttu-id="c4ecf-1034">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1034">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="c4ecf-1035">AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1035">AKS</span></span>

* <span data-ttu-id="c4ecf-1036">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1036">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="c4ecf-1037">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1037">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="c4ecf-1038">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1038">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="c4ecf-1039">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1039">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="c4ecf-1040">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1040">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1041">AppService</span></span>

* <span data-ttu-id="c4ecf-1042">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1042">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c4ecf-1043">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1043">June 5, 2018</span></span>

<span data-ttu-id="c4ecf-1044">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1044">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1045">Interactive</span></span>

* <span data-ttu-id="c4ecf-1046">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1046">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c4ecf-1047">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1047">June 5, 2018</span></span>

<span data-ttu-id="c4ecf-1048">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1048">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1049">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1049">Core</span></span>

* <span data-ttu-id="c4ecf-1050">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1050">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="c4ecf-1051">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1051">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1052">ACR</span></span>

* <span data-ttu-id="c4ecf-1053">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1053">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="c4ecf-1054">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1054">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="c4ecf-1055">AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1055">AKS</span></span>

* <span data-ttu-id="c4ecf-1056">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1056">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1057">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1057">Batch</span></span>

* <span data-ttu-id="c4ecf-1058">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1058">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-1059">IOT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1059">IOT</span></span>

* <span data-ttu-id="c4ecf-1060">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1060">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1061">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1061">Network</span></span>

* <span data-ttu-id="c4ecf-1062">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1062">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c4ecf-1063">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1063">Policy Insights</span></span>

* <span data-ttu-id="c4ecf-1064">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1064">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="c4ecf-1065">ARM</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1065">ARM</span></span>

* <span data-ttu-id="c4ecf-1066">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1066">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1067">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1067">SQL</span></span>

* <span data-ttu-id="c4ecf-1068">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1068">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="c4ecf-1069">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1069">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="c4ecf-1070">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1070">Storage</span></span>

* <span data-ttu-id="c4ecf-1071">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1071">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1072">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1072">VM</span></span>

* <span data-ttu-id="c4ecf-1073">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1073">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="c4ecf-1074">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1074">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="c4ecf-1075">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1075">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="c4ecf-1076">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1076">May 22, 2018</span></span>

<span data-ttu-id="c4ecf-1077">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1077">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1078">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1078">Core</span></span>

* <span data-ttu-id="c4ecf-1079">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1079">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1080">ACS</span></span>

* <span data-ttu-id="c4ecf-1081">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1081">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="c4ecf-1082">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1082">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1083">AppService</span></span>

* <span data-ttu-id="c4ecf-1084">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1084">Improved generic update commands</span></span>
* <span data-ttu-id="c4ecf-1085">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1085">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1086">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1086">Container</span></span>

* <span data-ttu-id="c4ecf-1087">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1087">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="c4ecf-1088">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1088">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1089">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1089">Extension</span></span>

* <span data-ttu-id="c4ecf-1090">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1090">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1091">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1091">Interactive</span></span>

* <span data-ttu-id="c4ecf-1092">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1092">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="c4ecf-1093">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1093">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-1094">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1094">KeyVault</span></span>

* <span data-ttu-id="c4ecf-1095">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1095">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1096">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1096">Network</span></span>

* <span data-ttu-id="c4ecf-1097">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1097">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="c4ecf-1098">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1098">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1099">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1099">SQL</span></span>

* <span data-ttu-id="c4ecf-1100">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1100">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="c4ecf-1101">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1101">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="c4ecf-1102">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1102">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="c4ecf-1103">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1103">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="c4ecf-1104">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1104">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="c4ecf-1105">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1105">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="c4ecf-1106">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1106">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="c4ecf-1107">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1107">`edition`.</span></span> <span data-ttu-id="c4ecf-1108">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1108">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="c4ecf-1109">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1109">`elasticPoolName`.</span></span> <span data-ttu-id="c4ecf-1110">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1110">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="c4ecf-1111">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1111">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="c4ecf-1112">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1112">`edition`.</span></span> <span data-ttu-id="c4ecf-1113">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1113">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="c4ecf-1114">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1114">`dtu`.</span></span> <span data-ttu-id="c4ecf-1115">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1115">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="c4ecf-1116">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1116">`databaseDtuMin`.</span></span> <span data-ttu-id="c4ecf-1117">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1117">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="c4ecf-1118">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1118">`databaseDtuMax`.</span></span> <span data-ttu-id="c4ecf-1119">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1119">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="c4ecf-1120">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1120">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="c4ecf-1121">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1121">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1122">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1122">Storage</span></span>

* <span data-ttu-id="c4ecf-1123">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1123">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="c4ecf-1124">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1124">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1125">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1125">VM</span></span>

* <span data-ttu-id="c4ecf-1126">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1126">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="c4ecf-1127">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1127">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="c4ecf-1128">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1128">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="c4ecf-1129">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1129">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="c4ecf-1130">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1130">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="c4ecf-1131">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1131">May 7, 2018</span></span>

<span data-ttu-id="c4ecf-1132">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1132">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1133">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1133">Core</span></span>

* <span data-ttu-id="c4ecf-1134">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1134">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="c4ecf-1135">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1135">Added limited support for positional arguments</span></span>
* <span data-ttu-id="c4ecf-1136">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1136">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="c4ecf-1137">#5591</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1137">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="c4ecf-1138">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1138">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="c4ecf-1139">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1139">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="c4ecf-1140">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1140">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="c4ecf-1141">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1141">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="c4ecf-1142">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1142">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1143">ACR</span></span>

* <span data-ttu-id="c4ecf-1144">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1144">Added ACR Build commands</span></span>
* <span data-ttu-id="c4ecf-1145">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1145">Improved resource not found error messages</span></span>
* <span data-ttu-id="c4ecf-1146">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1146">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="c4ecf-1147">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1147">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="c4ecf-1148">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1148">Improved repository commands error messages</span></span>
* <span data-ttu-id="c4ecf-1149">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1149">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1150">ACS</span></span>

* <span data-ttu-id="c4ecf-1151">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1151">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="c4ecf-1152">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1152">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="c4ecf-1153">AMS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1153">AMS</span></span>

* <span data-ttu-id="c4ecf-1154">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1154">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1155">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1155">Appservice</span></span>

* <span data-ttu-id="c4ecf-1156">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1156">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="c4ecf-1157">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1157">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="c4ecf-1158">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1158">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="c4ecf-1159">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1159">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4ecf-1160">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1160">Batch AI</span></span>

* <span data-ttu-id="c4ecf-1161">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1161">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4ecf-1162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1162">Cognitive Services</span></span>

* <span data-ttu-id="c4ecf-1163">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1163">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-1164">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1164">Consumption</span></span>

* <span data-ttu-id="c4ecf-1165">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1165">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1166">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1166">Container</span></span>

* <span data-ttu-id="c4ecf-1167">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1167">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c4ecf-1168">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1168">Cosmos DB</span></span>

* <span data-ttu-id="c4ecf-1169">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1169">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="c4ecf-1170">DMS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1170">DMS</span></span>

* <span data-ttu-id="c4ecf-1171">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1171">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1172">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1172">Extension</span></span>

* <span data-ttu-id="c4ecf-1173">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1173">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1174">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1174">Interactive</span></span>

* <span data-ttu-id="c4ecf-1175">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1175">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="c4ecf-1176">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1176">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="c4ecf-1177">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1177">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="c4ecf-1178">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1178">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="c4ecf-1179">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1179">Lab</span></span>

* <span data-ttu-id="c4ecf-1180">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1180">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1181">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1181">Network</span></span>

* <span data-ttu-id="c4ecf-1182">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1182">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="c4ecf-1183">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1183">Profile</span></span>

* <span data-ttu-id="c4ecf-1184">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1184">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="c4ecf-1185">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1185">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="c4ecf-1186">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1186">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="c4ecf-1187">Redis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1187">Redis</span></span>

* <span data-ttu-id="c4ecf-1188">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1188">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="c4ecf-1189">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1189">Deprecated `redis list-all`.</span></span> <span data-ttu-id="c4ecf-1190">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1190">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="c4ecf-1191">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1191">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="c4ecf-1192">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1192">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1193">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1193">Role</span></span>

* <span data-ttu-id="c4ecf-1194">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1194">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1195">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1195">Storage</span></span>

* <span data-ttu-id="c4ecf-1196">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1196">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="c4ecf-1197">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1197">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="c4ecf-1198">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1198">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="c4ecf-1199">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1199">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="c4ecf-1200">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1200">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1201">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1201">VM</span></span>

* <span data-ttu-id="c4ecf-1202">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1202">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="c4ecf-1203">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1203">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="c4ecf-1204">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1204">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="c4ecf-1205">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1205">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="c4ecf-1206">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1206">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="c4ecf-1207">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1207">Added write accelerator support</span></span>
* <span data-ttu-id="c4ecf-1208">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1208">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="c4ecf-1209">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1209">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="c4ecf-1210">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1210">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="c4ecf-1211">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1211">April 10, 2018</span></span>

<span data-ttu-id="c4ecf-1212">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1212">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1213">ACR</span></span>

* <span data-ttu-id="c4ecf-1214">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1214">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1215">ACS</span></span>

* <span data-ttu-id="c4ecf-1216">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1216">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1217">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1217">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="c4ecf-1219">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1219">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="c4ecf-1220">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1220">BatchAI</span></span>

* <span data-ttu-id="c4ecf-1221">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1221">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="c4ecf-1222">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1222">Job level mounting</span></span>
  - <span data-ttu-id="c4ecf-1223">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1223">Environment variables with secret values</span></span>
  - <span data-ttu-id="c4ecf-1224">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1224">Performance counters settings</span></span>
  - <span data-ttu-id="c4ecf-1225">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1225">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="c4ecf-1226">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1226">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="c4ecf-1227">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1227">Usage and limits reporting</span></span>
  - <span data-ttu-id="c4ecf-1228">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1228">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="c4ecf-1229">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1229">Support for custom images</span></span>
  - <span data-ttu-id="c4ecf-1230">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1230">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="c4ecf-1231">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1231">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="c4ecf-1232">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1232">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="c4ecf-1233">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1233">National clouds are supported</span></span>
* <span data-ttu-id="c4ecf-1234">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1234">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="c4ecf-1235">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1235">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="c4ecf-1236">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1236">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="c4ecf-1237">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1237">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="c4ecf-1238">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1238">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="c4ecf-1239">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1239">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="c4ecf-1240">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1240">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="c4ecf-1241">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1241">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="c4ecf-1242">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1242">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="c4ecf-1243">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1243">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="c4ecf-1244">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1244">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="c4ecf-1245">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1245">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="c4ecf-1246">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1246">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="c4ecf-1247">Facturation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1247">Billing</span></span>

* <span data-ttu-id="c4ecf-1248">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1248">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-1249">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1249">Consumption</span></span>

* <span data-ttu-id="c4ecf-1250">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1250">Added `marketplace` commands</span></span>
* <span data-ttu-id="c4ecf-1251">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1251">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="c4ecf-1252">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1252">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="c4ecf-1253">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1253">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="c4ecf-1254">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1254">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="c4ecf-1255">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1255">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1256">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1256">Container</span></span>

* <span data-ttu-id="c4ecf-1257">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1257">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="c4ecf-1258">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1258">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1259">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1259">Extension</span></span>

* <span data-ttu-id="c4ecf-1260">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1260">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1261">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1261">Interactive</span></span>

* <span data-ttu-id="c4ecf-1262">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1262">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="c4ecf-1263">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1263">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="c4ecf-1264">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1264">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1265">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1265">Network</span></span>

* <span data-ttu-id="c4ecf-1266">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1266">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="c4ecf-1267">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1267">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="c4ecf-1268">#4910</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1268">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="c4ecf-1269">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1269">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="c4ecf-1270">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1270">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="c4ecf-1271">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1271">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1272">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1272">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1273">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1273">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1274">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1274">Profile</span></span>

* <span data-ttu-id="c4ecf-1275">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1275">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="c4ecf-1276">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1276">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-1277">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1277">RDBMS</span></span>

* <span data-ttu-id="c4ecf-1278">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1278">Added `georestore` command</span></span>
* <span data-ttu-id="c4ecf-1279">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1279">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1280">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1280">Resource</span></span>

* <span data-ttu-id="c4ecf-1281">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1281">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="c4ecf-1282">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1282">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1283">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1283">SQL</span></span>

* <span data-ttu-id="c4ecf-1284">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1284">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1285">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1285">Storage</span></span>

* <span data-ttu-id="c4ecf-1286">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1286">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1287">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1287">VM</span></span>

* <span data-ttu-id="c4ecf-1288">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1288">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="c4ecf-1289">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1289">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="c4ecf-1291">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1291">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="c4ecf-1292">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1292">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="c4ecf-1293">#5718</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1293">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="c4ecf-1294">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1294">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="c4ecf-1295">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1295">March 27, 2018</span></span>

<span data-ttu-id="c4ecf-1296">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1296">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1297">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1297">Core</span></span>

* <span data-ttu-id="c4ecf-1298">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1298">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1299">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1299">ACS</span></span>

* <span data-ttu-id="c4ecf-1300">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1300">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1301">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1301">Appservice</span></span>

* <span data-ttu-id="c4ecf-1302">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1302">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="c4ecf-1303">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1303">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c4ecf-1304">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1304">Backup</span></span>

* <span data-ttu-id="c4ecf-1305">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1305">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="c4ecf-1306">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1306">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="c4ecf-1307">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1307">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="c4ecf-1308">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1308">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1309">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1309">Container</span></span>

* <span data-ttu-id="c4ecf-1310">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1310">Added `container exec` command.</span></span> <span data-ttu-id="c4ecf-1311">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1311">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="c4ecf-1312">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1312">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1313">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1313">Extension</span></span>

* <span data-ttu-id="c4ecf-1314">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1314">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="c4ecf-1315">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1315">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="c4ecf-1316">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1316">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1317">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1317">Interactive</span></span>

* <span data-ttu-id="c4ecf-1318">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1318">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="c4ecf-1319">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1319">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="c4ecf-1320">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1320">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="c4ecf-1321">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1321">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="c4ecf-1322">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1322">Lab</span></span>

* <span data-ttu-id="c4ecf-1323">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1323">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1324">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1324">Monitor</span></span>

* <span data-ttu-id="c4ecf-1325">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1325">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="c4ecf-1326">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1326">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="c4ecf-1327">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1327">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1328">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1328">Network</span></span>

* <span data-ttu-id="c4ecf-1329">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1329">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1330">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1330">Profile</span></span>

* <span data-ttu-id="c4ecf-1331">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1331">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-1332">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1332">RDBMS</span></span>

* <span data-ttu-id="c4ecf-1333">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1333">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1334">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1334">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="c4ecf-1336">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1336">Role</span></span>

* <span data-ttu-id="c4ecf-1337">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1337">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="c4ecf-1338">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1338">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="c4ecf-1339">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1339">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="c4ecf-1340">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1340">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="c4ecf-1341">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1341">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1342">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1342">Storage</span></span>

* <span data-ttu-id="c4ecf-1343">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1343">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="c4ecf-1344">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1344">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1345">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1345">VM</span></span>

* <span data-ttu-id="c4ecf-1346">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1346">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="c4ecf-1347">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1347">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="c4ecf-1348">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1348">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="c4ecf-1349">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1349">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="c4ecf-1350">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1350">March 13, 2018</span></span>

<span data-ttu-id="c4ecf-1351">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1351">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1352">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1352">ACR</span></span>

* <span data-ttu-id="c4ecf-1353">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1353">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="c4ecf-1354">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1354">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="c4ecf-1355">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1355">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1356">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1356">ACS</span></span>

* <span data-ttu-id="c4ecf-1357">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1357">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="c4ecf-1358">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1358">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="c4ecf-1359">Advisor</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1359">Advisor</span></span>

* <span data-ttu-id="c4ecf-1360">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1360">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="c4ecf-1361">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1361">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="c4ecf-1362">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1362">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="c4ecf-1363">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1363">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="c4ecf-1364">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1364">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1365">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1365">Appservice</span></span>

* <span data-ttu-id="c4ecf-1366">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1366">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="c4ecf-1367">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1367">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c4ecf-1368">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1368">Eventhubs</span></span>

* <span data-ttu-id="c4ecf-1369">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1369">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1370">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1370">Extension</span></span>

* <span data-ttu-id="c4ecf-1371">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1371">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1372">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1372">Interactive</span></span>

* <span data-ttu-id="c4ecf-1373">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1373">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="c4ecf-1374">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1374">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="c4ecf-1375">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1375">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="c4ecf-1376">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1376">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1377">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1377">Monitor</span></span>

* <span data-ttu-id="c4ecf-1378">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1378">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="c4ecf-1379">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1379">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="c4ecf-1380">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1380">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="c4ecf-1381">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1381">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1382">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1382">Network</span></span>

* <span data-ttu-id="c4ecf-1383">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1383">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="c4ecf-1384">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1384">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="c4ecf-1385">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1385">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="c4ecf-1386">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1386">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1387">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1387">Profile</span></span>

* <span data-ttu-id="c4ecf-1388">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1388">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="c4ecf-1389">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1389">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-1390">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1390">RDBMS</span></span>

* <span data-ttu-id="c4ecf-1391">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1391">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="c4ecf-1392">Service Bus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1392">Service Bus</span></span>

* <span data-ttu-id="c4ecf-1393">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1393">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1394">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1394">Storage</span></span>

* <span data-ttu-id="c4ecf-1395">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1395">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="c4ecf-1396">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1396">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1397">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1397">VM</span></span>

* <span data-ttu-id="c4ecf-1398">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1398">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="c4ecf-1399">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1399">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="c4ecf-1400">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1400">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="c4ecf-1401">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1401">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="c4ecf-1402">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1402">February 27, 2018</span></span>

<span data-ttu-id="c4ecf-1403">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1403">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1404">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1404">Core</span></span>

* <span data-ttu-id="c4ecf-1405">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1405">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="c4ecf-1406">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1406">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="c4ecf-1407">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1407">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1408">ACS</span></span>

* <span data-ttu-id="c4ecf-1409">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1409">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="c4ecf-1410">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1410">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="c4ecf-1411">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1411">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="c4ecf-1412">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1412">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1413">Appservice</span></span>

* <span data-ttu-id="c4ecf-1414">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1414">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="c4ecf-1415">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1415">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4ecf-1416">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1416">Cognitive Services</span></span>

* <span data-ttu-id="c4ecf-1417">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1417">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-1418">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1418">Consumption</span></span>

* <span data-ttu-id="c4ecf-1419">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1419">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="c4ecf-1420">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1420">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1421">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1421">Container</span></span>

* <span data-ttu-id="c4ecf-1422">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1422">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1423">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1423">Network</span></span>

* <span data-ttu-id="c4ecf-1424">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1424">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1425">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1425">Resource</span></span>

* <span data-ttu-id="c4ecf-1426">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1426">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1427">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1427">Role</span></span>

* <span data-ttu-id="c4ecf-1428">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1428">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1429">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1429">SQL</span></span>

* <span data-ttu-id="c4ecf-1430">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1430">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1431">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1431">Storage</span></span>

* <span data-ttu-id="c4ecf-1432">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1432">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1433">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1433">VM</span></span>

* <span data-ttu-id="c4ecf-1434">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1434">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="c4ecf-1435">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1435">February 13, 2018</span></span>

<span data-ttu-id="c4ecf-1436">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1436">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1437">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1437">Core</span></span>

* <span data-ttu-id="c4ecf-1438">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1438">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1439">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1439">ACS</span></span>

* <span data-ttu-id="c4ecf-1440">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1440">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="c4ecf-1441">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1441">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="c4ecf-1442">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1442">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="c4ecf-1443">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1443">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="c4ecf-1444">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1444">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="c4ecf-1445">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1445">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="c4ecf-1446">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1446">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="c4ecf-1447">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1447">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1448">Appservice</span></span>

* <span data-ttu-id="c4ecf-1449">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1449">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="c4ecf-1450">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1450">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1451">CDN</span></span>

* <span data-ttu-id="c4ecf-1452">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1452">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1453">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1453">Container</span></span>

* <span data-ttu-id="c4ecf-1454">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1454">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="c4ecf-1455">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1455">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-1456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1456">CosmosDB</span></span>

* <span data-ttu-id="c4ecf-1457">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1457">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1458">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1458">Extension</span></span>

* <span data-ttu-id="c4ecf-1459">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1459">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="c4ecf-1460">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1460">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="c4ecf-1461">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1461">Feedback</span></span>

* <span data-ttu-id="c4ecf-1462">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1462">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1463">Interactive</span></span>

* <span data-ttu-id="c4ecf-1464">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1464">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="c4ecf-1465">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1465">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-1466">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1466">IoT</span></span>

* <span data-ttu-id="c4ecf-1467">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1467">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c4ecf-1468">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1468">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c4ecf-1469">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1469">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1470">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1470">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1471">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1471">Monitor</span></span>

* <span data-ttu-id="c4ecf-1472">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1472">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1473">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1473">Network</span></span>

* <span data-ttu-id="c4ecf-1474">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1474">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="c4ecf-1475">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1475">Profile</span></span>

* <span data-ttu-id="c4ecf-1476">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1476">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1477">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1477">Resource</span></span>

* <span data-ttu-id="c4ecf-1478">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1478">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1479">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1479">Role</span></span>

* <span data-ttu-id="c4ecf-1480">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1480">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1481">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1481">SQL</span></span>

* <span data-ttu-id="c4ecf-1482">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1482">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="c4ecf-1483">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1483">Added `sql db rename`</span></span>
* <span data-ttu-id="c4ecf-1484">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1484">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1485">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1485">Storage</span></span>

* <span data-ttu-id="c4ecf-1486">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1486">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1487">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1487">VM</span></span>

* <span data-ttu-id="c4ecf-1488">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1488">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="c4ecf-1489">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1489">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="c4ecf-1490">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1490">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="c4ecf-1491">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1491">January 31, 2018</span></span>

<span data-ttu-id="c4ecf-1492">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1492">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1493">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1493">Core</span></span>

* <span data-ttu-id="c4ecf-1494">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1494">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="c4ecf-1495">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1495">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="c4ecf-1496">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1496">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="c4ecf-1497">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1497">Use `--verbose` to see</span></span>
* <span data-ttu-id="c4ecf-1498">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1498">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1499">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1499">ACS</span></span>

* <span data-ttu-id="c4ecf-1500">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1500">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="c4ecf-1501">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1501">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1502">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1502">Appservice</span></span>

* <span data-ttu-id="c4ecf-1503">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1503">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="c4ecf-1504">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1504">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-1505">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1505">CDN</span></span>

* <span data-ttu-id="c4ecf-1506">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1506">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-1507">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1507">CosmosDB</span></span>

* <span data-ttu-id="c4ecf-1508">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1508">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1509">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1509">Interactive</span></span>

* <span data-ttu-id="c4ecf-1510">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1510">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1511">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1511">Network</span></span>

* <span data-ttu-id="c4ecf-1512">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1512">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="c4ecf-1513">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1513">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="c4ecf-1514">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1514">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="c4ecf-1515">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1515">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="c4ecf-1516">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1516">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="c4ecf-1517">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1517">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="c4ecf-1518">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1518">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="c4ecf-1519">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1519">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="c4ecf-1520">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1520">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="c4ecf-1521">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1521">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1522">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1522">Profile</span></span>

* <span data-ttu-id="c4ecf-1523">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1523">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1524">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1524">Resource</span></span>

* <span data-ttu-id="c4ecf-1525">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1525">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1526">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1526">Storage</span></span>

* <span data-ttu-id="c4ecf-1527">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1527">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="c4ecf-1528">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1528">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="c4ecf-1529">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1529">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="c4ecf-1530">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1530">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="c4ecf-1531">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1531">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1532">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1532">VM</span></span>

* <span data-ttu-id="c4ecf-1533">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1533">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="c4ecf-1534">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1534">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="c4ecf-1535">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1535">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="c4ecf-1536">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1536">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="c4ecf-1537">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1537">January 17, 2018</span></span>

<span data-ttu-id="c4ecf-1538">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1538">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1539">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1539">ACR</span></span>

* <span data-ttu-id="c4ecf-1540">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1540">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="c4ecf-1541">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1541">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1542">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1542">ACS</span></span>

* <span data-ttu-id="c4ecf-1543">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1543">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="c4ecf-1544">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1544">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1545">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1545">Appservice</span></span>

* <span data-ttu-id="c4ecf-1546">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1546">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="c4ecf-1547">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1547">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="c4ecf-1548">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1548">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="c4ecf-1549">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1549">Backup</span></span>

* <span data-ttu-id="c4ecf-1550">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1550">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="c4ecf-1551">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1551">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="c4ecf-1552">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1552">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="c4ecf-1553">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1553">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="c4ecf-1554">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1554">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1555">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1555">Batch</span></span>

* <span data-ttu-id="c4ecf-1556">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1556">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="c4ecf-1557">Cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1557">Cloud</span></span>

* <span data-ttu-id="c4ecf-1558">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1558">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-1559">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1559">Consumption</span></span>

* <span data-ttu-id="c4ecf-1560">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1560">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4ecf-1561">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1561">Event Grid</span></span>

* <span data-ttu-id="c4ecf-1562">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1562">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c4ecf-1563">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1563">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c4ecf-1564">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1564">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="c4ecf-1565">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="c4ecf-1566">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1566">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="c4ecf-1567">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1567">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="c4ecf-1568">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1568">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="c4ecf-1569">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1569">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-1570">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1570">Interactive</span></span>

* <span data-ttu-id="c4ecf-1571">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1571">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="c4ecf-1572">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1572">Fixed errors on startup</span></span>
* <span data-ttu-id="c4ecf-1573">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1573">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-1574">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1574">IoT</span></span>

* <span data-ttu-id="c4ecf-1575">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1575">Added support for device provisioning service</span></span>
* <span data-ttu-id="c4ecf-1576">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1576">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="c4ecf-1577">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1577">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1578">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1578">Monitor</span></span>

* <span data-ttu-id="c4ecf-1579">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1579">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="c4ecf-1580">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1580">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="c4ecf-1581">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1581">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1582">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1582">Network</span></span>

* <span data-ttu-id="c4ecf-1583">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1583">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="c4ecf-1584">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1584">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1585">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1585">Profile</span></span>

* <span data-ttu-id="c4ecf-1586">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1586">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1587">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1587">Role</span></span>

* <span data-ttu-id="c4ecf-1588">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1588">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4ecf-1589">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1589">Service Fabric</span></span>

* <span data-ttu-id="c4ecf-1590">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1590">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="c4ecf-1591">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1591">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1592">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1592">VM</span></span>

* <span data-ttu-id="c4ecf-1593">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1593">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="c4ecf-1594">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1594">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="c4ecf-1595">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1595">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="c4ecf-1596">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1596">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="c4ecf-1597">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1597">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="c4ecf-1598">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1598">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4ecf-1599">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1599">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4ecf-1600">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1600">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="c4ecf-1601">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1601">December 19, 2017</span></span>

<span data-ttu-id="c4ecf-1602">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1602">Version 2.0.23</span></span>

* <span data-ttu-id="c4ecf-1603">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1603">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1604">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1604">Container</span></span>

* <span data-ttu-id="c4ecf-1605">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1605">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1606">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1606">Network</span></span>

* <span data-ttu-id="c4ecf-1607">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1607">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1608">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1608">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1609">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1609">Storage</span></span>

* <span data-ttu-id="c4ecf-1610">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1610">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1611">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1611">VM</span></span>

* <span data-ttu-id="c4ecf-1612">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1612">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="c4ecf-1613">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1613">December 5, 2017</span></span>

<span data-ttu-id="c4ecf-1614">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1614">Version 2.0.22</span></span>

* <span data-ttu-id="c4ecf-1615">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1615">Removed `az component` commands.</span></span> <span data-ttu-id="c4ecf-1616">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1616">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1617">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1617">Core</span></span>
* <span data-ttu-id="c4ecf-1618">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1618">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="c4ecf-1619">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1619">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1620">ACS</span></span>

* <span data-ttu-id="c4ecf-1621">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1621">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="c4ecf-1622">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1622">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="c4ecf-1623">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1623">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="c4ecf-1624">Advisor</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1624">Advisor</span></span>

* <span data-ttu-id="c4ecf-1625">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1625">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1626">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1626">Appservice</span></span>

* <span data-ttu-id="c4ecf-1627">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1627">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="c4ecf-1628">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1628">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="c4ecf-1629">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1629">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="c4ecf-1630">Consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1630">Consumption</span></span>

* <span data-ttu-id="c4ecf-1631">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1631">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1632">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1632">Container</span></span>

* <span data-ttu-id="c4ecf-1633">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1633">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1634">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1634">Monitor</span></span>

* <span data-ttu-id="c4ecf-1635">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1635">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1636">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1636">Resource</span></span>

* <span data-ttu-id="c4ecf-1637">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1637">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-1638">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1638">Role</span></span>

* <span data-ttu-id="c4ecf-1639">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1639">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="c4ecf-1640">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1640">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="c4ecf-1641">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1641">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1642">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1642">SQL</span></span>

* <span data-ttu-id="c4ecf-1643">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1643">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="c4ecf-1644">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1644">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1645">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1645">VM</span></span>

* <span data-ttu-id="c4ecf-1646">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1646">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="c4ecf-1647">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1647">November 14, 2017</span></span>

<span data-ttu-id="c4ecf-1648">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1648">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1649">ACR</span></span>

* <span data-ttu-id="c4ecf-1650">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1650">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="c4ecf-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1651">ACS</span></span>

* <span data-ttu-id="c4ecf-1652">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1652">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="c4ecf-1653">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1653">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="c4ecf-1654">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1654">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="c4ecf-1655">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1655">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="c4ecf-1656">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1656">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1657">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1657">Appservice</span></span>

* <span data-ttu-id="c4ecf-1658">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1658">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="c4ecf-1659">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1659">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="c4ecf-1660">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1660">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="c4ecf-1661">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1661">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="c4ecf-1662">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1662">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="c4ecf-1663">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1663">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1664">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1664">Batch</span></span>

* <span data-ttu-id="c4ecf-1665">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1665">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="c4ecf-1666">Batchai</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1666">Batchai</span></span>

* <span data-ttu-id="c4ecf-1667">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1667">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="c4ecf-1668">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1668">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="c4ecf-1669">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1669">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="c4ecf-1670">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1670">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="c4ecf-1671">Cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1671">Cloud</span></span>

* <span data-ttu-id="c4ecf-1672">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1672">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1673">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1673">Container</span></span>

* <span data-ttu-id="c4ecf-1674">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1674">Added support to open multiple ports</span></span>
* <span data-ttu-id="c4ecf-1675">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1675">Added container group restart policy</span></span>
* <span data-ttu-id="c4ecf-1676">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1676">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="c4ecf-1677">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1677">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4ecf-1678">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1678">Data Lake Analytics</span></span>

* <span data-ttu-id="c4ecf-1679">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1679">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4ecf-1680">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1680">Data Lake Store</span></span>

* <span data-ttu-id="c4ecf-1681">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1681">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1682">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1682">Extension</span></span>

* <span data-ttu-id="c4ecf-1683">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1683">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="c4ecf-1684">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1684">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-1685">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1685">IoT</span></span>

* <span data-ttu-id="c4ecf-1686">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1686">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1687">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1687">Monitor</span></span>

* <span data-ttu-id="c4ecf-1688">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1688">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1689">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1689">Network</span></span>

* <span data-ttu-id="c4ecf-1690">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1690">Added support for CAA DNS records</span></span>
* <span data-ttu-id="c4ecf-1691">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1691">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="c4ecf-1692">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1692">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="c4ecf-1693">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1693">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="c4ecf-1694">Réservations</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1694">Reservations</span></span>

* <span data-ttu-id="c4ecf-1695">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1695">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1696">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1696">Resource</span></span>

* <span data-ttu-id="c4ecf-1697">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1697">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1698">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1698">SQL</span></span>

* <span data-ttu-id="c4ecf-1699">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1699">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1700">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1700">Storage</span></span>

* <span data-ttu-id="c4ecf-1701">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1701">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="c4ecf-1702">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1702">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="c4ecf-1703">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1703">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="c4ecf-1704">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1704">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="c4ecf-1705">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1705">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="c4ecf-1706">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1706">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="c4ecf-1707">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1707">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1708">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1708">VM</span></span>

* <span data-ttu-id="c4ecf-1709">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1709">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="c4ecf-1710">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1710">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="c4ecf-1711">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1711">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="c4ecf-1712">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1712">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="c4ecf-1713">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1713">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c4ecf-1714">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1714">October 24, 2017</span></span>

<span data-ttu-id="c4ecf-1715">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1715">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1716">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1716">Core</span></span>

* <span data-ttu-id="c4ecf-1717">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1717">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1718">ACR</span></span>

* <span data-ttu-id="c4ecf-1719">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1719">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c4ecf-1720">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1720">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c4ecf-1721">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1721">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1722">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1722">ACS</span></span>

* <span data-ttu-id="c4ecf-1723">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1723">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c4ecf-1724">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1724">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1725">Appservice</span></span>

* <span data-ttu-id="c4ecf-1726">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1726">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c4ecf-1727">Composant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1727">Component</span></span>

* <span data-ttu-id="c4ecf-1728">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1728">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-1729">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1729">Monitor</span></span>

* <span data-ttu-id="c4ecf-1730">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1730">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1731">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1731">Resource</span></span>

* <span data-ttu-id="c4ecf-1732">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1732">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c4ecf-1733">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1733">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1734">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1734">VM</span></span>

* <span data-ttu-id="c4ecf-1735">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1735">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c4ecf-1736">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1736">October 9, 2017</span></span>

<span data-ttu-id="c4ecf-1737">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1737">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1738">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1738">Core</span></span>

* <span data-ttu-id="c4ecf-1739">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1739">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1740">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1740">Appservice</span></span>

* <span data-ttu-id="c4ecf-1741">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1741">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1742">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1742">Batch</span></span>

* <span data-ttu-id="c4ecf-1743">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1743">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c4ecf-1744">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1744">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c4ecf-1745">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1745">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c4ecf-1746">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1746">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c4ecf-1747">Batchai</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1747">Batchai</span></span>

* <span data-ttu-id="c4ecf-1748">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1748">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-1749">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1749">Keyvault</span></span>

* <span data-ttu-id="c4ecf-1750">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1750">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c4ecf-1751">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1751">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c4ecf-1752">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1752">Network</span></span>

* <span data-ttu-id="c4ecf-1753">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1753">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c4ecf-1754">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1754">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1755">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1755">Resource</span></span>

* <span data-ttu-id="c4ecf-1756">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1756">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c4ecf-1757">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1757">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c4ecf-1758">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1758">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c4ecf-1759">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1759">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1760">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1760">Sql</span></span>

* <span data-ttu-id="c4ecf-1761">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1761">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c4ecf-1762">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1762">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c4ecf-1763">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1763">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1764">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1764">Storage</span></span>

* <span data-ttu-id="c4ecf-1765">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1765">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1766">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1766">Vm</span></span>

* <span data-ttu-id="c4ecf-1767">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1767">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c4ecf-1768">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1768">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c4ecf-1769">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1769">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c4ecf-1770">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1770">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c4ecf-1771">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1771">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c4ecf-1772">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1772">September 22, 2017</span></span>

<span data-ttu-id="c4ecf-1773">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1773">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1774">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1774">Resource</span></span>

* <span data-ttu-id="c4ecf-1775">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1775">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c4ecf-1776">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1776">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c4ecf-1777">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1777">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c4ecf-1778">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1778">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1779">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1779">Network</span></span>

* <span data-ttu-id="c4ecf-1780">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1780">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c4ecf-1781">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1781">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c4ecf-1782">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1782">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c4ecf-1783">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1783">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c4ecf-1784">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1784">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1785">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1785">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1786">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1786">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1787">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1787">Storage</span></span>

* <span data-ttu-id="c4ecf-1788">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1788">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c4ecf-1789">Événement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1789">Eventgrid</span></span>

* <span data-ttu-id="c4ecf-1790">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1790">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1791">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1791">SQL</span></span>

* <span data-ttu-id="c4ecf-1792">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1792">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c4ecf-1793">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1793">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c4ecf-1794">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1794">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-1795">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1795">Keyvault</span></span>

* <span data-ttu-id="c4ecf-1796">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1796">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1797">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1797">VM</span></span>

* <span data-ttu-id="c4ecf-1798">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1798">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c4ecf-1799">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1799">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c4ecf-1800">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1800">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c4ecf-1801">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1801">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c4ecf-1802">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1802">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c4ecf-1803">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1803">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1804">ACS</span></span>

* <span data-ttu-id="c4ecf-1805">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1805">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1806">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1806">Appservice</span></span>

* <span data-ttu-id="c4ecf-1807">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1807">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c4ecf-1808">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1808">Backup</span></span>

* <span data-ttu-id="c4ecf-1809">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1809">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c4ecf-1810">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1810">September 11, 2017</span></span>

<span data-ttu-id="c4ecf-1811">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1811">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c4ecf-1812">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1812">Core</span></span>

* <span data-ttu-id="c4ecf-1813">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1813">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c4ecf-1814">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1814">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1815">Acs</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1815">Acs</span></span>

* <span data-ttu-id="c4ecf-1816">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1816">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c4ecf-1817">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1817">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1818">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1818">Appservice</span></span>

* <span data-ttu-id="c4ecf-1819">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1819">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-1820">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1820">CDN</span></span>

* <span data-ttu-id="c4ecf-1821">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1821">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="c4ecf-1822">Extension</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1822">Extension</span></span>

* <span data-ttu-id="c4ecf-1823">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1823">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-1824">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1824">Keyvault</span></span>

* <span data-ttu-id="c4ecf-1825">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1825">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1826">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1826">Network</span></span>

* <span data-ttu-id="c4ecf-1827">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1827">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c4ecf-1828">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1828">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c4ecf-1829">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1829">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c4ecf-1830">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1830">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c4ecf-1831">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1831">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-1832">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1832">Resource</span></span>

* <span data-ttu-id="c4ecf-1833">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1833">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c4ecf-1834">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1834">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c4ecf-1835">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1835">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c4ecf-1836">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1836">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1837">SQL</span></span>

* <span data-ttu-id="c4ecf-1838">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1838">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1839">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1839">VM</span></span>

* <span data-ttu-id="c4ecf-1840">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1840">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c4ecf-1841">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1841">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c4ecf-1842">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1842">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c4ecf-1843">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1843">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c4ecf-1844">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1844">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c4ecf-1845">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1845">August 31, 2017</span></span>

<span data-ttu-id="c4ecf-1846">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1846">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-1847">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1847">Keyvault</span></span>

* <span data-ttu-id="c4ecf-1848">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1848">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c4ecf-1849">Sf</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1849">Sf</span></span>

* <span data-ttu-id="c4ecf-1850">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1850">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1851">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1851">Storage</span></span>

* <span data-ttu-id="c4ecf-1852">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1852">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c4ecf-1853">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1853">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c4ecf-1854">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1854">August 28, 2017</span></span>

<span data-ttu-id="c4ecf-1855">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1855">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c4ecf-1856">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1856">CLI</span></span>

* <span data-ttu-id="c4ecf-1857">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1857">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1858">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1858">ACS</span></span>

* <span data-ttu-id="c4ecf-1859">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1859">Corrected preview regions</span></span>
* <span data-ttu-id="c4ecf-1860">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1860">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="c4ecf-1861">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1861">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1862">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1862">Appservice</span></span>

* <span data-ttu-id="c4ecf-1863">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1863">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c4ecf-1864">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1864">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c4ecf-1865">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1865">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c4ecf-1866">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1866">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c4ecf-1867">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1867">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-1868">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1868">IoT</span></span>

* <span data-ttu-id="c4ecf-1869">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1869">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1870">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1870">Network</span></span>

* <span data-ttu-id="c4ecf-1871">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1871">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c4ecf-1872">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1872">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1873">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1873">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c4ecf-1874">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1874">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c4ecf-1875">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1875">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1876">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1876">Profile</span></span>

* <span data-ttu-id="c4ecf-1877">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1877">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4ecf-1878">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1878">Service Fabric</span></span>

* <span data-ttu-id="c4ecf-1879">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1879">Preview release</span></span>
* <span data-ttu-id="c4ecf-1880">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1880">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c4ecf-1881">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1881">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c4ecf-1882">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1882">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1883">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1883">Storage</span></span>

* <span data-ttu-id="c4ecf-1884">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1884">Enabled setting blob tier</span></span>
* <span data-ttu-id="c4ecf-1885">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1885">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c4ecf-1886">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1886">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="c4ecf-1887">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1887">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c4ecf-1888">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1888">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c4ecf-1889">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1889">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1890">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1890">VM</span></span>

* <span data-ttu-id="c4ecf-1891">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1891">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c4ecf-1892">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1892">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="c4ecf-1893">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1893">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4ecf-1894">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1894">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c4ecf-1895">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1895">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c4ecf-1896">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1896">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c4ecf-1897">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1897">August 15, 2017</span></span>

<span data-ttu-id="c4ecf-1898">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1898">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1899">ACS</span></span>

* <span data-ttu-id="c4ecf-1900">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1900">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1901">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1901">Appservice</span></span>

* <span data-ttu-id="c4ecf-1902">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1902">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4ecf-1903">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1903">Event Grid</span></span>

* <span data-ttu-id="c4ecf-1904">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1904">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c4ecf-1905">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1905">August 11, 2017</span></span>

<span data-ttu-id="c4ecf-1906">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1906">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1907">ACS</span></span>

* <span data-ttu-id="c4ecf-1908">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1908">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1909">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1909">Batch</span></span>

* <span data-ttu-id="c4ecf-1910">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1910">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c4ecf-1911">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1911">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c4ecf-1912">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1912">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c4ecf-1913">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1913">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c4ecf-1914">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1914">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c4ecf-1915">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1915">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c4ecf-1916">Composant</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1916">Component</span></span>

* <span data-ttu-id="c4ecf-1917">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1917">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c4ecf-1918">Conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1918">Container</span></span>

* <span data-ttu-id="c4ecf-1919">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1919">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c4ecf-1920">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1920">Data Lake Store</span></span>

* <span data-ttu-id="c4ecf-1921">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1921">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4ecf-1922">Event Grid</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1922">Event Grid</span></span>

* <span data-ttu-id="c4ecf-1923">Version initiale</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1923">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-1924">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1924">Network</span></span>

* <span data-ttu-id="c4ecf-1925">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1925">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c4ecf-1926">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1926">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c4ecf-1927">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1927">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c4ecf-1928">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1928">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-1929">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1929">Profile</span></span>

* <span data-ttu-id="c4ecf-1930">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1930">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-1931">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1931">Storage</span></span>

* <span data-ttu-id="c4ecf-1932">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1932">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-1933">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1933">VM</span></span>

* <span data-ttu-id="c4ecf-1934">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1934">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c4ecf-1935">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1935">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c4ecf-1936">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1936">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c4ecf-1937">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1937">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c4ecf-1938">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1938">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c4ecf-1939">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1939">July 28, 2017</span></span>

<span data-ttu-id="c4ecf-1940">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1940">Version 2.0.12</span></span>

* <span data-ttu-id="c4ecf-1941">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1941">Added container commands</span></span>
* <span data-ttu-id="c4ecf-1942">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1942">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c4ecf-1943">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1943">Core</span></span>

* <span data-ttu-id="c4ecf-1944">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1944">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c4ecf-1945">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1945">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c4ecf-1946">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1946">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c4ecf-1947">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1947">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c4ecf-1948">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1948">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c4ecf-1949">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1949">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c4ecf-1950">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1950">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c4ecf-1951">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1951">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c4ecf-1952">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1952">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c4ecf-1953">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1953">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c4ecf-1954">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1954">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c4ecf-1955">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1955">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c4ecf-1956">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1956">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c4ecf-1957">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1957">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c4ecf-1958">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1958">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c4ecf-1959">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1959">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c4ecf-1960">ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1960">ACR</span></span>

* <span data-ttu-id="c4ecf-1961">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1961">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c4ecf-1962">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1962">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c4ecf-1963">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1963">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c4ecf-1964">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1964">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c4ecf-1965">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1965">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c4ecf-1966">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1966">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1967">ACS</span></span>

* <span data-ttu-id="c4ecf-1968">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1968">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-1969">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1969">Appservice</span></span>

* <span data-ttu-id="c4ecf-1970">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1970">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c4ecf-1971">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1971">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c4ecf-1972">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1972">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c4ecf-1973">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1973">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c4ecf-1974">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1974">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c4ecf-1975">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1975">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c4ecf-1976">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1976">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c4ecf-1977">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1977">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c4ecf-1978">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1978">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c4ecf-1979">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1979">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c4ecf-1980">Batch</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1980">Batch</span></span>

* <span data-ttu-id="c4ecf-1981">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1981">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c4ecf-1982">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1982">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c4ecf-1983">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1983">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c4ecf-1984">CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1984">CDN</span></span>

* <span data-ttu-id="c4ecf-1985">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1985">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="c4ecf-1986">Cloud</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1986">Cloud</span></span>

* <span data-ttu-id="c4ecf-1987">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1987">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c4ecf-1988">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1988">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c4ecf-1989">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1989">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c4ecf-1990">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1990">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c4ecf-1991">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1991">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-1992">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1992">CosmosDB</span></span>

* <span data-ttu-id="c4ecf-1993">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1993">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c4ecf-1994">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1994">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4ecf-1995">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1995">Data Lake Analytics</span></span>

* <span data-ttu-id="c4ecf-1996">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1996">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c4ecf-1997">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1997">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c4ecf-1998">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1998">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4ecf-1999">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-1999">Data Lake Store</span></span>

* <span data-ttu-id="c4ecf-2000">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2000">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c4ecf-2001">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2001">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c4ecf-2002">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2002">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c4ecf-2003">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2003">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c4ecf-2004">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2004">Interactive</span></span>

* <span data-ttu-id="c4ecf-2005">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2005">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c4ecf-2006">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2006">Increased test coverage</span></span>
* <span data-ttu-id="c4ecf-2007">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2007">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c4ecf-2008">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2008">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c4ecf-2009">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2009">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c4ecf-2010">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2010">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c4ecf-2011">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2011">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c4ecf-2012">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2012">Added `--progress` flag</span></span>
* <span data-ttu-id="c4ecf-2013">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2013">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c4ecf-2014">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2014">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c4ecf-2015">IoT</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2015">IoT</span></span>

* <span data-ttu-id="c4ecf-2016">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2016">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c4ecf-2017">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2017">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c4ecf-2018">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2018">Key vault</span></span>

* <span data-ttu-id="c4ecf-2019">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2019">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c4ecf-2020">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2020">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c4ecf-2021">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2021">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c4ecf-2022">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2022">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c4ecf-2023">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2023">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c4ecf-2024">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2024">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c4ecf-2025">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2025">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c4ecf-2026">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2026">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c4ecf-2027">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2027">Lab</span></span>

* <span data-ttu-id="c4ecf-2028">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2028">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c4ecf-2029">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2029">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-2030">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2030">Monitor</span></span>

* <span data-ttu-id="c4ecf-2031">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2031">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c4ecf-2032">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2032">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c4ecf-2033">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2033">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c4ecf-2034">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2034">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c4ecf-2035">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2035">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c4ecf-2036">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2036">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c4ecf-2037">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2037">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c4ecf-2038">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2038">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c4ecf-2039">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2039">`location` no longer required</span></span>
  * <span data-ttu-id="c4ecf-2040">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2040">Add name and ID support for target</span></span>
  * <span data-ttu-id="c4ecf-2041">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2041">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c4ecf-2042">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2042">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c4ecf-2043">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2043">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c4ecf-2044">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2044">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c4ecf-2045">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2045">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c4ecf-2046">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2046">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-2047">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2047">Network</span></span>

* <span data-ttu-id="c4ecf-2048">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2048">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c4ecf-2049">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2049">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c4ecf-2050">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2050">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c4ecf-2051">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2051">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c4ecf-2052">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2052">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c4ecf-2053">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2053">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c4ecf-2054">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2054">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c4ecf-2055">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2055">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c4ecf-2056">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2056">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c4ecf-2057">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2057">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c4ecf-2058">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2058">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c4ecf-2059">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2059">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c4ecf-2060">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2060">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c4ecf-2061">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2061">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c4ecf-2062">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2062">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c4ecf-2063">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2063">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c4ecf-2064">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2064">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c4ecf-2065">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2065">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c4ecf-2066">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2066">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c4ecf-2067">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2067">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c4ecf-2068">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2068">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c4ecf-2069">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2069">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c4ecf-2070">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2070">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c4ecf-2071">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2071">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c4ecf-2072">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2072">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c4ecf-2073">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2073">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c4ecf-2074">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2074">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-2075">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2075">Profile</span></span>

* <span data-ttu-id="c4ecf-2076">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2076">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c4ecf-2077">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2077">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c4ecf-2078">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2078">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c4ecf-2079">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2079">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c4ecf-2080">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2080">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4ecf-2081">SGBDR</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2081">RDBMS</span></span>

* <span data-ttu-id="c4ecf-2082">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2082">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c4ecf-2083">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2083">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c4ecf-2084">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2084">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c4ecf-2085">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2085">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-2086">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2086">Resource</span></span>

* <span data-ttu-id="c4ecf-2087">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2087">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c4ecf-2088">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2088">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c4ecf-2089">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2089">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c4ecf-2090">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2090">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c4ecf-2091">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2091">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c4ecf-2092">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2092">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c4ecf-2093">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2093">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c4ecf-2094">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2094">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-2095">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2095">Role</span></span>

* <span data-ttu-id="c4ecf-2096">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2096">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c4ecf-2097">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2097">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c4ecf-2098">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2098">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c4ecf-2099">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2099">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c4ecf-2100">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2100">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4ecf-2101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2101">Service Fabric</span></span>
* <span data-ttu-id="c4ecf-2102">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2102">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c4ecf-2103">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2103">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c4ecf-2104">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2104">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-2105">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2105">SQL</span></span>

* <span data-ttu-id="c4ecf-2106">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2106">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c4ecf-2107">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2107">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c4ecf-2108">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2108">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-2109">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2109">Storage</span></span>

* <span data-ttu-id="c4ecf-2110">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2110">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c4ecf-2111">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2111">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c4ecf-2112">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2112">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c4ecf-2113">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2113">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="c4ecf-2114">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2114">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="c4ecf-2115">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2115">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-2116">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2116">VM</span></span>

* <span data-ttu-id="c4ecf-2117">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2117">Support configuring nsg</span></span>
* <span data-ttu-id="c4ecf-2118">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2118">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c4ecf-2119">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2119">Support managed service identities</span></span>
* <span data-ttu-id="c4ecf-2120">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2120">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="c4ecf-2121">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2121">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c4ecf-2122">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2122">May 10, 2017</span></span>

<span data-ttu-id="c4ecf-2123">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2123">Version 2.0.6</span></span>

* <span data-ttu-id="c4ecf-2124">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2124">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c4ecf-2125">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2125">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c4ecf-2126">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2126">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="c4ecf-2127">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2127">Include Cognitive Services module</span></span>
* <span data-ttu-id="c4ecf-2128">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2128">Include Service Fabric module</span></span>
* <span data-ttu-id="c4ecf-2129">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2129">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="c4ecf-2130">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2130">Add support for CDN commands</span></span>
* <span data-ttu-id="c4ecf-2131">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2131">Remove Container module</span></span>
* <span data-ttu-id="c4ecf-2132">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2132">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c4ecf-2133">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2133">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c4ecf-2134">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2134">Core</span></span>

* <span data-ttu-id="c4ecf-2135">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2135">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="c4ecf-2136">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2136">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c4ecf-2137">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2137">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c4ecf-2138">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2138">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c4ecf-2139">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2139">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c4ecf-2140">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2140">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c4ecf-2141">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2141">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c4ecf-2142">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2142">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c4ecf-2143">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2143">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c4ecf-2144">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2144">core: Improved performance</span></span>
* <span data-ttu-id="c4ecf-2145">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2145">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c4ecf-2146">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2146">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2147">ACS</span></span>

* <span data-ttu-id="c4ecf-2148">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2148">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c4ecf-2149">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2149">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c4ecf-2150">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2150">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c4ecf-2151">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2151">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-2152">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2152">AppService</span></span>

* <span data-ttu-id="c4ecf-2153">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2153">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c4ecf-2154">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2154">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c4ecf-2155">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2155">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c4ecf-2156">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2156">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c4ecf-2157">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2157">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c4ecf-2158">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2158">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c4ecf-2159">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2159">support slot swap with preview</span></span>
* <span data-ttu-id="c4ecf-2160">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2160">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c4ecf-2161">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2161">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4ecf-2162">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2162">CosmosDB</span></span>

* <span data-ttu-id="c4ecf-2163">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2163">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="c4ecf-2164">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2164">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c4ecf-2165">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2165">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c4ecf-2166">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2166">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4ecf-2167">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2167">Data Lake Analytics</span></span>

* <span data-ttu-id="c4ecf-2168">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2168">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="c4ecf-2169">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2169">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c4ecf-2170">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2170">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c4ecf-2171">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2171">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c4ecf-2172">Table</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2172">Table</span></span>
  * <span data-ttu-id="c4ecf-2173">Fonction table</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2173">Table valued function</span></span>
  * <span data-ttu-id="c4ecf-2174">Affichage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2174">View</span></span>
  * <span data-ttu-id="c4ecf-2175">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2175">Table Statistics.</span></span> <span data-ttu-id="c4ecf-2176">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2176">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4ecf-2177">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2177">Data Lake Store</span></span>

* <span data-ttu-id="c4ecf-2178">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2178">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="c4ecf-2179">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2179">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c4ecf-2180">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2180">missed help for access show.</span></span> <span data-ttu-id="c4ecf-2181">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2181">adding it.</span></span> <span data-ttu-id="c4ecf-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c4ecf-2183">Rechercher</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2183">Find</span></span>

* <span data-ttu-id="c4ecf-2184">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2184">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4ecf-2185">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2185">KeyVault</span></span>

* <span data-ttu-id="c4ecf-2186">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2186">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c4ecf-2187">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2187">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="c4ecf-2188">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2188">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c4ecf-2189">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2189">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="c4ecf-2190">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2190">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c4ecf-2191">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2191">Lab</span></span>

* <span data-ttu-id="c4ecf-2192">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2192">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="c4ecf-2193">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2193">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="c4ecf-2194">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2194">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="c4ecf-2195">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2195">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="c4ecf-2196">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2196">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="c4ecf-2197">Surveiller</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2197">Monitor</span></span>

* <span data-ttu-id="c4ecf-2198">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2198">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c4ecf-2199">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2199">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c4ecf-2200">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2200">Network</span></span>

* <span data-ttu-id="c4ecf-2201">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2201">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="c4ecf-2202">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2202">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="c4ecf-2203">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2203">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="c4ecf-2204">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2204">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="c4ecf-2205">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2205">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="c4ecf-2206">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2206">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="c4ecf-2207">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2207">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="c4ecf-2208">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2208">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="c4ecf-2209">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2209">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="c4ecf-2210">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2210">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c4ecf-2211">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2211">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="c4ecf-2212">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2212">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="c4ecf-2213">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2213">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="c4ecf-2214">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2214">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="c4ecf-2215">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2215">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="c4ecf-2216">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2216">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="c4ecf-2217">Profil</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2217">Profile</span></span>

* <span data-ttu-id="c4ecf-2218">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2218">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c4ecf-2219">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2219">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c4ecf-2220">Redis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2220">Redis</span></span>

* <span data-ttu-id="c4ecf-2221">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2221">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c4ecf-2222">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2222">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="c4ecf-2223">Ressource</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2223">Resource</span></span>

* <span data-ttu-id="c4ecf-2224">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2224">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c4ecf-2225">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2225">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c4ecf-2226">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2226">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c4ecf-2227">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2227">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c4ecf-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c4ecf-2229">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2229">Add docs for az lock update.</span></span> <span data-ttu-id="c4ecf-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c4ecf-2231">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2231">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c4ecf-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c4ecf-2233">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2233">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c4ecf-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c4ecf-2235">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2235">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c4ecf-2236">Rôle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2236">Role</span></span>

* <span data-ttu-id="c4ecf-2237">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2237">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c4ecf-2238">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2238">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c4ecf-2239">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2239">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c4ecf-2240">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2240">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c4ecf-2241">SQL</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2241">SQL</span></span>

* <span data-ttu-id="c4ecf-2242">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2242">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="c4ecf-2243">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2243">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c4ecf-2244">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2244">Storage</span></span>

* <span data-ttu-id="c4ecf-2245">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2245">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="c4ecf-2246">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2246">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c4ecf-2247">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2247">Add support for large block blob upload</span></span>
* <span data-ttu-id="c4ecf-2248">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2248">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-2249">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2249">VM</span></span>

* <span data-ttu-id="c4ecf-2250">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2250">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c4ecf-2251">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2251">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c4ecf-2252">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2252">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c4ecf-2253">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2253">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c4ecf-2254">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2254">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c4ecf-2255">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2255">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c4ecf-2256">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2256">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c4ecf-2257">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2257">April 3, 2017</span></span>

<span data-ttu-id="c4ecf-2258">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2258">Version 2.0.2</span></span>

<span data-ttu-id="c4ecf-2259">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2259">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="c4ecf-2260">Principal</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2260">Core</span></span>

* <span data-ttu-id="c4ecf-2261">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2261">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="c4ecf-2262">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2262">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c4ecf-2263">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2263">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c4ecf-2264">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2264">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c4ecf-2265">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2265">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c4ecf-2266">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2266">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c4ecf-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c4ecf-2268">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2268">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c4ecf-2269">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2269">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="c4ecf-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2270">ACS</span></span>

* <span data-ttu-id="c4ecf-2271">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2271">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c4ecf-2272">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2272">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c4ecf-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c4ecf-2274">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2274">Add support for windows clusters.</span></span> <span data-ttu-id="c4ecf-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c4ecf-2276">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2276">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c4ecf-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="c4ecf-2278">AppService</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2278">AppService</span></span>

* <span data-ttu-id="c4ecf-2279">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2279">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c4ecf-2280">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2280">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c4ecf-2281">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2281">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c4ecf-2282">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2282">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="c4ecf-2283">DataLake</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2283">DataLake</span></span>

* <span data-ttu-id="c4ecf-2284">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2284">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="c4ecf-2285">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2285">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="c4ecf-2286">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2286">DocuemntDB</span></span>

* <span data-ttu-id="c4ecf-2287">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2287">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c4ecf-2288">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2288">VM</span></span>

* <span data-ttu-id="c4ecf-2289">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2289">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c4ecf-2290">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2290">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c4ecf-2291">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2291">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c4ecf-2292">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2292">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c4ecf-2293">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2293">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c4ecf-2294">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2294">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="c4ecf-2295">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2295">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c4ecf-2296">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2296">February 27, 2017</span></span>

<span data-ttu-id="c4ecf-2297">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2297">Version 2.0.0</span></span>

<span data-ttu-id="c4ecf-2298">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2298">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="c4ecf-2299">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2299">Container Service (acs)</span></span>
- <span data-ttu-id="c4ecf-2300">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2300">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c4ecf-2301">Réseau</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2301">Networking</span></span>
- <span data-ttu-id="c4ecf-2302">Stockage</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2302">Storage</span></span>

<span data-ttu-id="c4ecf-2303">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2303">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="c4ecf-2304">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2304">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="c4ecf-2305">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2305">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="c4ecf-2306">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2306">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="c4ecf-2307">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2307">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="c4ecf-2308">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2308">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c4ecf-2309">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2309">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c4ecf-2310">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2310">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="c4ecf-2311">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c4ecf-2311">Provide feedback from the command line with the `az feedback` command</span></span>

