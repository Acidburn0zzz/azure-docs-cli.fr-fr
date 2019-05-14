---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/06/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ce11abccc23ee1f150916ef2f91dc895d4664d31
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240506"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="2a9cf-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-103">Azure CLI release notes</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="2a9cf-104">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-104">May 6, 2019</span></span>

<span data-ttu-id="2a9cf-105">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="2a9cf-105">Version 2.0.64</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-106">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-106">Appservice</span></span>
* <span data-ttu-id="2a9cf-107">Dépréciation de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-107">Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="2a9cf-108">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-108">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="2a9cf-109">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-109">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="2a9cf-110">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="2a9cf-110">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="2a9cf-111">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-111">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="2a9cf-112">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-112">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="2a9cf-113">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="2a9cf-113">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="2a9cf-114">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-114">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="2a9cf-115">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-115">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="2a9cf-116">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-116">Added `create-remote-connection` command</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-117">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-117">Role</span></span>
* <span data-ttu-id="2a9cf-118">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-118">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="2a9cf-119">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-119">April 23, 2019</span></span>

<span data-ttu-id="2a9cf-120">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="2a9cf-120">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-121">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-121">ACS</span></span>
* <span data-ttu-id="2a9cf-122">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-122">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="2a9cf-123">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-123">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-124">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-124">AMS</span></span>
* <span data-ttu-id="2a9cf-125">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-125">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-126">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-126">AppService</span></span>
* <span data-ttu-id="2a9cf-127">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-127">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="2a9cf-128">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="2a9cf-128">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="2a9cf-129">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="2a9cf-129">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="2a9cf-130">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="2a9cf-130">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="2a9cf-131">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="2a9cf-131">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="2a9cf-132">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-132">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="2a9cf-133">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="2a9cf-133">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="2a9cf-134">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-134">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="2a9cf-135">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-135">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="2a9cf-136">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-136">Deployment Manager</span></span>
* <span data-ttu-id="2a9cf-137">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="2a9cf-137">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="2a9cf-138">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-138">Lab</span></span>
* <span data-ttu-id="2a9cf-139">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-139">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-140">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-140">Network</span></span>
* <span data-ttu-id="2a9cf-141">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-141">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-142">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-142">Resource</span></span>
* <span data-ttu-id="2a9cf-143">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-143">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="2a9cf-144">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-144">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="2a9cf-145">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-145">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="2a9cf-146">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-146">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-147">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-147">SQL</span></span>
* <span data-ttu-id="2a9cf-148">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-148">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="2a9cf-149">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-149">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="2a9cf-150">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-150">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="2a9cf-151">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-151">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-152">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-152">Storage</span></span>
* <span data-ttu-id="2a9cf-153">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-153">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-154">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-154">VM</span></span>
* <span data-ttu-id="2a9cf-155">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="2a9cf-155">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="2a9cf-156">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="2a9cf-156">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="2a9cf-157">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="2a9cf-157">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="2a9cf-158">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-158">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-159">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-159">Core</span></span>
* <span data-ttu-id="2a9cf-160">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="2a9cf-160">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-161">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-161">ACR</span></span>
* <span data-ttu-id="2a9cf-162">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-162">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-163">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-163">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="2a9cf-166">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-166">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="2a9cf-167">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-167">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-168">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-168">AppService</span></span>
* <span data-ttu-id="2a9cf-169">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-169">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="2a9cf-170">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-170">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="2a9cf-171">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-171">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="2a9cf-172">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="2a9cf-172">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="2a9cf-173">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-173">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="2a9cf-174">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-174">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="2a9cf-175">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="2a9cf-175">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-176">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-176">CDN</span></span>
* <span data-ttu-id="2a9cf-177">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-177">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="2a9cf-178">Commentaires</span><span class="sxs-lookup"><span data-stu-id="2a9cf-178">Feedback</span></span>
* <span data-ttu-id="2a9cf-179">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="2a9cf-179">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="2a9cf-180">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="2a9cf-180">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="2a9cf-181">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="2a9cf-181">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-182">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-182">Monitor</span></span>
* <span data-ttu-id="2a9cf-183">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-183">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="2a9cf-184">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-184">Network</span></span>
* <span data-ttu-id="2a9cf-185">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-185">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="2a9cf-186">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-186">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="2a9cf-187">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-187">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="2a9cf-188">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-188">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="2a9cf-189">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-189">PrivateDNS</span></span>
* <span data-ttu-id="2a9cf-190">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-190">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-191">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-191">Resource</span></span>
* <span data-ttu-id="2a9cf-192">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-192">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-193">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-193">Role</span></span>
* <span data-ttu-id="2a9cf-194">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-194">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="2a9cf-195">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-195">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-196">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-196">SQL</span></span>
* <span data-ttu-id="2a9cf-197">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="2a9cf-197">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-198">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-198">Storage</span></span>
* <span data-ttu-id="2a9cf-199">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-199">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="2a9cf-200">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-200">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="2a9cf-201">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="2a9cf-201">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="2a9cf-202">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-202">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="2a9cf-203">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-203">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="2a9cf-204">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-204">Core</span></span>
* <span data-ttu-id="2a9cf-205">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-205">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="2a9cf-206">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-206">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="2a9cf-207">Cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-207">Cloud</span></span>
* <span data-ttu-id="2a9cf-208">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-208">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-209">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-209">ACR</span></span>
* <span data-ttu-id="2a9cf-210">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="2a9cf-210">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="2a9cf-211">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-211">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="2a9cf-212">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="2a9cf-212">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="2a9cf-213">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-213">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-214">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-214">AppService</span></span>
* <span data-ttu-id="2a9cf-215">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-215">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="2a9cf-216">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-216">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="2a9cf-217">Service BOT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-217">BOT Service</span></span>
* <span data-ttu-id="2a9cf-218">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-218">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="2a9cf-219">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="2a9cf-219">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="2a9cf-220">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-220">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="2a9cf-221">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="2a9cf-221">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-222">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-222">CDN</span></span>
* <span data-ttu-id="2a9cf-223">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-223">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="2a9cf-224">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-224">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="2a9cf-225">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="2a9cf-225">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="2a9cf-226">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-226">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-227">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="2a9cf-227">Cosmosdb</span></span>
* <span data-ttu-id="2a9cf-228">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-228">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="2a9cf-229">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-229">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-230">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-230">Interactive</span></span>
* <span data-ttu-id="2a9cf-231">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="2a9cf-231">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-232">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-232">Monitor</span></span>
* <span data-ttu-id="2a9cf-233">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-233">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-234">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-234">Network</span></span>
* <span data-ttu-id="2a9cf-235">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-235">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-236">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-236">Profile</span></span>
* <span data-ttu-id="2a9cf-237">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-237">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="2a9cf-238">Postgres</span><span class="sxs-lookup"><span data-stu-id="2a9cf-238">Postgres</span></span> 
* <span data-ttu-id="2a9cf-239">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="2a9cf-239">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="2a9cf-240">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-240">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-241">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-241">Resource</span></span>
* <span data-ttu-id="2a9cf-242">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-242">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="2a9cf-243">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-243">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="2a9cf-244">Graph</span><span class="sxs-lookup"><span data-stu-id="2a9cf-244">Graph</span></span>
* <span data-ttu-id="2a9cf-245">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-245">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="2a9cf-246">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-246">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="2a9cf-247">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-247">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="2a9cf-248">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-248">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="2a9cf-249">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="2a9cf-249">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-250">storage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-250">storage</span></span>
* <span data-ttu-id="2a9cf-251">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-251">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="2a9cf-252">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="2a9cf-252">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="2a9cf-253">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-253">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="2a9cf-254">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-254">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-255">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-255">VM</span></span>
* <span data-ttu-id="2a9cf-256">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-256">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="2a9cf-257">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-257">March 12, 2019</span></span>

<span data-ttu-id="2a9cf-258">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="2a9cf-258">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-259">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-259">Core</span></span>

* <span data-ttu-id="2a9cf-260">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="2a9cf-260">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-261">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-261">ACR</span></span>

* <span data-ttu-id="2a9cf-262">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="2a9cf-262">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-263">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-263">ACS</span></span>

* <span data-ttu-id="2a9cf-264">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="2a9cf-264">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="2a9cf-265">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-265">AppService</span></span>

* <span data-ttu-id="2a9cf-266">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="2a9cf-266">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="2a9cf-267">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-267">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="2a9cf-268">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-268">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="2a9cf-269">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-269">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="2a9cf-270">Botservice</span><span class="sxs-lookup"><span data-stu-id="2a9cf-270">Botservice</span></span>

* <span data-ttu-id="2a9cf-271">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="2a9cf-271">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="2a9cf-272">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="2a9cf-272">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="2a9cf-273">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-273">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="2a9cf-274">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="2a9cf-274">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-275">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-275">Container</span></span>

* <span data-ttu-id="2a9cf-276">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-276">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="2a9cf-277">Event Hub</span><span class="sxs-lookup"><span data-stu-id="2a9cf-277">EventHub</span></span>

* <span data-ttu-id="2a9cf-278">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="2a9cf-278">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="2a9cf-279">Rechercher</span><span class="sxs-lookup"><span data-stu-id="2a9cf-279">Find</span></span>

* <span data-ttu-id="2a9cf-280">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="2a9cf-280">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2a9cf-281">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2a9cf-281">HDInsight</span></span>

* <span data-ttu-id="2a9cf-282">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-282">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-283">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-283">Network</span></span>

* <span data-ttu-id="2a9cf-284">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="2a9cf-284">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-285">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2a9cf-285">Rdbms</span></span>

* <span data-ttu-id="2a9cf-286">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="2a9cf-286">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-287">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-287">Role</span></span>

* <span data-ttu-id="2a9cf-288">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-288">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="2a9cf-289">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="2a9cf-289">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2a9cf-290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2a9cf-290">Service Fabric</span></span>

* <span data-ttu-id="2a9cf-291">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="2a9cf-291">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="2a9cf-292">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-292">February 26, 2019</span></span>

<span data-ttu-id="2a9cf-293">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="2a9cf-293">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-294">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-294">Core</span></span>

* <span data-ttu-id="2a9cf-295">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-295">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-296">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-296">ACR</span></span>

* <span data-ttu-id="2a9cf-297">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-297">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="2a9cf-298">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="2a9cf-298">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-299">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-299">ACS</span></span>

* <span data-ttu-id="2a9cf-300">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-300">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-301">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-301">AppService</span></span>

* <span data-ttu-id="2a9cf-302">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-302">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-303">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-303">Batch</span></span>
* <span data-ttu-id="2a9cf-304">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-304">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="2a9cf-305">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-305">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="2a9cf-306">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="2a9cf-306">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="2a9cf-307">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-307">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="2a9cf-308">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="2a9cf-308">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="2a9cf-309">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-309">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-310">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-310">CosmosDB</span></span>

* <span data-ttu-id="2a9cf-311">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-311">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="2a9cf-312">Kusto</span><span class="sxs-lookup"><span data-stu-id="2a9cf-312">Kusto</span></span>

* <span data-ttu-id="2a9cf-313">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="2a9cf-313">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-314">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-314">Network</span></span>

* <span data-ttu-id="2a9cf-315">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-315">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="2a9cf-316">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-316">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="2a9cf-317">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-317">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="2a9cf-318">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-318">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="2a9cf-319">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-319">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="2a9cf-320">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-320">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="2a9cf-321">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-321">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-322">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-322">Resource</span></span>

* <span data-ttu-id="2a9cf-323">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-323">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="2a9cf-324">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-324">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="2a9cf-325">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-325">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="2a9cf-326">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-326">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="2a9cf-327">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-327">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-328">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-328">Role</span></span>

* <span data-ttu-id="2a9cf-329">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-329">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-330">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-330">VM</span></span>

* <span data-ttu-id="2a9cf-331">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-331">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="2a9cf-332">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-332">February 12, 2019</span></span>

<span data-ttu-id="2a9cf-333">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="2a9cf-333">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-334">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-334">Core</span></span>

* <span data-ttu-id="2a9cf-335">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="2a9cf-335">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="2a9cf-336">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="2a9cf-336">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-337">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-337">ACR</span></span>
* <span data-ttu-id="2a9cf-338">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-338">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="2a9cf-339">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-339">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-340">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-340">ACS</span></span>
* <span data-ttu-id="2a9cf-341">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-341">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="2a9cf-342">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-342">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="2a9cf-343">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-343">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-344">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-344">AMS</span></span>
* <span data-ttu-id="2a9cf-345">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-345">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="2a9cf-346">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-346">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-347">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-347">Appservice</span></span>
* <span data-ttu-id="2a9cf-348">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-348">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="2a9cf-349">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="2a9cf-349">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="2a9cf-350">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-350">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="2a9cf-351">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="2a9cf-351">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="2a9cf-352">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="2a9cf-352">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="2a9cf-353">Botservice</span><span class="sxs-lookup"><span data-stu-id="2a9cf-353">Botservice</span></span>
* <span data-ttu-id="2a9cf-354">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-354">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="2a9cf-355">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-355">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="2a9cf-356">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-356">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="2a9cf-357">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="2a9cf-357">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="2a9cf-358">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-358">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="2a9cf-359">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="2a9cf-359">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="2a9cf-360">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-360">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="2a9cf-361">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="2a9cf-361">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="2a9cf-362">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-362">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="2a9cf-363">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="2a9cf-363">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="2a9cf-364">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-364">Key Vault</span></span>
* <span data-ttu-id="2a9cf-365">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-365">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-366">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-366">Monitor</span></span>
* <span data-ttu-id="2a9cf-367">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-367">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-368">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-368">Network</span></span>
* <span data-ttu-id="2a9cf-369">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="2a9cf-369">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="2a9cf-370">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="2a9cf-370">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="2a9cf-371">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-371">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="2a9cf-372">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-372">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="2a9cf-373">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="2a9cf-373">Policy Insights</span></span>
* <span data-ttu-id="2a9cf-374">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="2a9cf-374">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-375">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-375">RDBMS</span></span>
* <span data-ttu-id="2a9cf-376">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-376">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="2a9cf-377">Redis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-377">Redis</span></span>
* <span data-ttu-id="2a9cf-378">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-378">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="2a9cf-379">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-379">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="2a9cf-380">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-380">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="2a9cf-381">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="2a9cf-381">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="2a9cf-382">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-382">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="2a9cf-383">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-383">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="2a9cf-384">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-384">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-385">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-385">Role</span></span>
* <span data-ttu-id="2a9cf-386">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-386">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="2a9cf-387">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-387">SQL VM</span></span>
* <span data-ttu-id="2a9cf-388">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-388">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-389">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-389">VM</span></span>
* <span data-ttu-id="2a9cf-390">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-390">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="2a9cf-391">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-391">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="2a9cf-392">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="2a9cf-392">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="2a9cf-393">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-393">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="2a9cf-394">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-394">January 31, 2019</span></span>

<span data-ttu-id="2a9cf-395">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="2a9cf-395">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-396">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-396">Core</span></span>

* <span data-ttu-id="2a9cf-397">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="2a9cf-397">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="2a9cf-398">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-398">January 28, 2019</span></span>

<span data-ttu-id="2a9cf-399">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="2a9cf-399">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-400">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-400">ACR</span></span>
* <span data-ttu-id="2a9cf-401">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="2a9cf-401">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-402">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-402">ACS</span></span>
* <span data-ttu-id="2a9cf-403">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="2a9cf-403">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="2a9cf-404">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-404">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="2a9cf-405">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-405">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-406">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-406">AMS</span></span>
* <span data-ttu-id="2a9cf-407">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-407">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="2a9cf-408">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-408">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-409">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-409">Appservice</span></span>
* <span data-ttu-id="2a9cf-410">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-410">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="2a9cf-411">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="2a9cf-411">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="2a9cf-412">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="2a9cf-412">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-413">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-413">Container</span></span>
* <span data-ttu-id="2a9cf-414">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-414">Added `container start` command</span></span>
* <span data-ttu-id="2a9cf-415">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-415">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2a9cf-416">EventGrid</span><span class="sxs-lookup"><span data-stu-id="2a9cf-416">EventGrid</span></span>
* <span data-ttu-id="2a9cf-417">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-417">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="2a9cf-418">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-418">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="2a9cf-419">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="2a9cf-419">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="2a9cf-420">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-420">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="2a9cf-421">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-421">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2a9cf-422">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2a9cf-422">HDInsight</span></span>
* <span data-ttu-id="2a9cf-423">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-423">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="2a9cf-424">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="2a9cf-424">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="2a9cf-425">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-425">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="2a9cf-426">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-426">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="2a9cf-427">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-427">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="2a9cf-428">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-428">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-429">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-429">IoT</span></span>
* <span data-ttu-id="2a9cf-430">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="2a9cf-430">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="2a9cf-431">Kusto</span><span class="sxs-lookup"><span data-stu-id="2a9cf-431">Kusto</span></span>
* <span data-ttu-id="2a9cf-432">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-432">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-433">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-433">Monitor</span></span>
* <span data-ttu-id="2a9cf-434">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-434">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-435">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-435">Profile</span></span>
* <span data-ttu-id="2a9cf-436">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-436">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-437">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-437">Network</span></span>
* <span data-ttu-id="2a9cf-438">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="2a9cf-438">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="2a9cf-439">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="2a9cf-439">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-440">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-440">Resource</span></span>
* <span data-ttu-id="2a9cf-441">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-441">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="2a9cf-442">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-442">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="2a9cf-443">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-443">SQL Virtual Machine</span></span>
* <span data-ttu-id="2a9cf-444">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-444">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-445">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-445">Storage</span></span>
* <span data-ttu-id="2a9cf-446">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="2a9cf-446">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="2a9cf-447">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-447">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-448">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-448">VM</span></span>
* <span data-ttu-id="2a9cf-449">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-449">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="2a9cf-450">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-450">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="2a9cf-451">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="2a9cf-451">January 15, 2019</span></span>

<span data-ttu-id="2a9cf-452">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="2a9cf-452">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-453">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-453">ACR</span></span>
* <span data-ttu-id="2a9cf-454">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-454">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="2a9cf-455">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="2a9cf-455">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="2a9cf-456">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-456">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="2a9cf-457">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-457">ACS</span></span>
* <span data-ttu-id="2a9cf-458">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-458">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-459">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-459">Appservice</span></span>
* <span data-ttu-id="2a9cf-460">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="2a9cf-460">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="2a9cf-461">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-461">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="2a9cf-462">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-462">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="2a9cf-463">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-463">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="2a9cf-464">Botservice</span><span class="sxs-lookup"><span data-stu-id="2a9cf-464">Botservice</span></span>
* <span data-ttu-id="2a9cf-465">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-465">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="2a9cf-466">Configuration</span><span class="sxs-lookup"><span data-stu-id="2a9cf-466">Configure</span></span>
* <span data-ttu-id="2a9cf-467">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="2a9cf-467">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-468">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-468">CosmosDB</span></span>
* <span data-ttu-id="2a9cf-469">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-469">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2a9cf-470">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2a9cf-470">HDInsight</span></span>
* <span data-ttu-id="2a9cf-471">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="2a9cf-471">Added commands for managing applications</span></span>
* <span data-ttu-id="2a9cf-472">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="2a9cf-472">Added commands for managing script actions</span></span>
* <span data-ttu-id="2a9cf-473">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-473">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="2a9cf-474">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-474">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="2a9cf-475">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-475">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-476">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-476">Network</span></span>
* <span data-ttu-id="2a9cf-477">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-477">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="2a9cf-478">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="2a9cf-478">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="2a9cf-479">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-479">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="2a9cf-480">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-480">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-481">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-481">Role</span></span>
* <span data-ttu-id="2a9cf-482">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-482">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="2a9cf-483">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="2a9cf-483">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="2a9cf-484">Sécurité</span><span class="sxs-lookup"><span data-stu-id="2a9cf-484">Security</span></span>
* <span data-ttu-id="2a9cf-485">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-485">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-486">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-486">Storage</span></span>
* <span data-ttu-id="2a9cf-487">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-487">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="2a9cf-488">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="2a9cf-488">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="2a9cf-489">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-489">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="2a9cf-490">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-490">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="2a9cf-491">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-491">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-492">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-492">VM</span></span>
* <span data-ttu-id="2a9cf-493">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="2a9cf-493">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="2a9cf-494">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-494">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="2a9cf-495">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-495">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="2a9cf-496">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-496">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="2a9cf-497">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-497">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="2a9cf-498">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="2a9cf-498">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="2a9cf-499">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-499">December 20, 2018</span></span>

<span data-ttu-id="2a9cf-500">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="2a9cf-500">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="2a9cf-501">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-501">Appservice</span></span>
* <span data-ttu-id="2a9cf-502">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-502">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="2a9cf-503">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="2a9cf-503">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="2a9cf-504">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-504">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="2a9cf-505">IotCentral</span><span class="sxs-lookup"><span data-stu-id="2a9cf-505">IoTCentral</span></span>
* <span data-ttu-id="2a9cf-506">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="2a9cf-506">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-507">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-507">Role</span></span>
* <span data-ttu-id="2a9cf-508">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-508">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-509">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-509">SQL</span></span>
* <span data-ttu-id="2a9cf-510">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-510">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-511">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-511">VM</span></span>
* <span data-ttu-id="2a9cf-512">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-512">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="2a9cf-513">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-513">December 18, 2018</span></span>

<span data-ttu-id="2a9cf-514">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="2a9cf-514">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="2a9cf-515">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-515">ACR</span></span>
* <span data-ttu-id="2a9cf-516">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-516">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="2a9cf-517">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="2a9cf-517">Condensed the table layout for task list</span></span>
* <span data-ttu-id="2a9cf-518">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="2a9cf-518">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-519">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-519">ACS</span></span>
* <span data-ttu-id="2a9cf-520">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="2a9cf-520">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="2a9cf-521">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-521">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="2a9cf-522">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-522">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="2a9cf-523">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-523">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="2a9cf-524">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-524">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="2a9cf-525">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="2a9cf-525">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-526">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-526">Appservice</span></span>
* <span data-ttu-id="2a9cf-527">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-527">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="2a9cf-528">Botservice</span><span class="sxs-lookup"><span data-stu-id="2a9cf-528">Botservice</span></span>
* <span data-ttu-id="2a9cf-529">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-529">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="2a9cf-530">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="2a9cf-530">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="2a9cf-531">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="2a9cf-531">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="2a9cf-532">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-532">Reduced Kudu network calls</span></span>
* <span data-ttu-id="2a9cf-533">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="2a9cf-533">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-534">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-534">Consumption</span></span>
* <span data-ttu-id="2a9cf-535">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="2a9cf-535">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-536">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-536">CosmosDB</span></span>
* <span data-ttu-id="2a9cf-537">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-537">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="2a9cf-538">Cartes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-538">Maps</span></span>
* <span data-ttu-id="2a9cf-539">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-539">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-540">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-540">Network</span></span>
* <span data-ttu-id="2a9cf-541">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-541">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="2a9cf-542">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-542">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-543">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-543">Resource</span></span>
* <span data-ttu-id="2a9cf-544">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-544">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="2a9cf-545">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-545">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-546">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-546">Storage</span></span>
*  <span data-ttu-id="2a9cf-547">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-547">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-548">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-548">VM</span></span>
* <span data-ttu-id="2a9cf-549">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-549">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="2a9cf-550">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-550">December 4, 2018</span></span>

<span data-ttu-id="2a9cf-551">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="2a9cf-551">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="2a9cf-552">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-552">Core</span></span>
* <span data-ttu-id="2a9cf-553">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-553">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="2a9cf-554">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-554">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-555">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-555">Appservice</span></span>
* <span data-ttu-id="2a9cf-556">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-556">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="2a9cf-557">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-557">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-558">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-558">Network</span></span>
* <span data-ttu-id="2a9cf-559">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="2a9cf-559">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-560">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-560">Role</span></span>
* <span data-ttu-id="2a9cf-561">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-561">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="2a9cf-562">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-562">VM</span></span>
* <span data-ttu-id="2a9cf-563">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-563">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="2a9cf-564">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-564">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="2a9cf-565">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-565">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="2a9cf-566">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-566">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="2a9cf-567">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-567">November 20, 2018</span></span>

<span data-ttu-id="2a9cf-568">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="2a9cf-568">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="2a9cf-569">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-569">Core</span></span>
* <span data-ttu-id="2a9cf-570">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="2a9cf-570">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-571">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-571">ACR</span></span>
* <span data-ttu-id="2a9cf-572">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="2a9cf-572">Added context token to task step</span></span>
* <span data-ttu-id="2a9cf-573">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="2a9cf-573">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="2a9cf-574">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-574">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-575">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-575">Appservice</span></span>
* <span data-ttu-id="2a9cf-576">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-576">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="2a9cf-577">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-577">Updated the default `node_version`.</span></span> <span data-ttu-id="2a9cf-578">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="2a9cf-578">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="2a9cf-579">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-579">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="2a9cf-580">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="2a9cf-580">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="2a9cf-581">IotCentral</span><span class="sxs-lookup"><span data-stu-id="2a9cf-581">IotCentral</span></span>
* <span data-ttu-id="2a9cf-582">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="2a9cf-582">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-583">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-583">KeyVault</span></span>
* <span data-ttu-id="2a9cf-584">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-584">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-585">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-585">Network</span></span>
* <span data-ttu-id="2a9cf-586">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="2a9cf-586">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="2a9cf-587">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-587">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="2a9cf-588">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-588">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="2a9cf-589">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-589">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-590">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2a9cf-590">Rdbms</span></span>
* <span data-ttu-id="2a9cf-591">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="2a9cf-591">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="2a9cf-592">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-592">Rbac</span></span>
* <span data-ttu-id="2a9cf-593">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-593">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="2a9cf-594">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-594">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="2a9cf-595">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-595">Storage</span></span>
* <span data-ttu-id="2a9cf-596">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-596">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="2a9cf-597">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-597">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="2a9cf-598">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-598">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="2a9cf-599">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-599">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-600">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-600">VM</span></span>
* <span data-ttu-id="2a9cf-601">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-601">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="2a9cf-602">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-602">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="2a9cf-603">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-603">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="2a9cf-604">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-604">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="2a9cf-605">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-605">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="2a9cf-606">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-606">Added `snapshot wait` command</span></span>
* <span data-ttu-id="2a9cf-607">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-607">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="2a9cf-608">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-608">November 6, 2018</span></span>

<span data-ttu-id="2a9cf-609">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="2a9cf-609">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-610">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-610">Core</span></span>
* <span data-ttu-id="2a9cf-611">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="2a9cf-611">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-612">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-612">ACR</span></span>
* <span data-ttu-id="2a9cf-613">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="2a9cf-613">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="2a9cf-614">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="2a9cf-614">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-615">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-615">ACS</span></span>
* <span data-ttu-id="2a9cf-616">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-616">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="2a9cf-617">Advisor</span><span class="sxs-lookup"><span data-stu-id="2a9cf-617">Advisor</span></span>
* <span data-ttu-id="2a9cf-618">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-618">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-619">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-619">AMS</span></span>
* <span data-ttu-id="2a9cf-620">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-620">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="2a9cf-621">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-621">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="2a9cf-622">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-622">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="2a9cf-623">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="2a9cf-623">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="2a9cf-624">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-624">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="2a9cf-625">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-625">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="2a9cf-626">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-626">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="2a9cf-627">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-627">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="2a9cf-628">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-628">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="2a9cf-629">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-629">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="2a9cf-630">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-630">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="2a9cf-631">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-631">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="2a9cf-632">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="2a9cf-632">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="2a9cf-633">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-633">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="2a9cf-634">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-634">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="2a9cf-635">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="2a9cf-635">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="2a9cf-636">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-636">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-637">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-637">AppService</span></span>
* <span data-ttu-id="2a9cf-638">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-638">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="2a9cf-639">Configuration</span><span class="sxs-lookup"><span data-stu-id="2a9cf-639">Configure</span></span>
* <span data-ttu-id="2a9cf-640">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-640">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-641">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-641">Container</span></span>
* <span data-ttu-id="2a9cf-642">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="2a9cf-642">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="2a9cf-643">Event Hub</span><span class="sxs-lookup"><span data-stu-id="2a9cf-643">EventHub</span></span>
* <span data-ttu-id="2a9cf-644">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-644">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-645">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-645">Interactive</span></span>
* <span data-ttu-id="2a9cf-646">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="2a9cf-646">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-647">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-647">Monitor</span></span>
* <span data-ttu-id="2a9cf-648">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-648">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-649">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-649">Network</span></span>
* <span data-ttu-id="2a9cf-650">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-650">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="2a9cf-651">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-651">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="2a9cf-652">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-652">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="2a9cf-653">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-653">Profile</span></span>
* <span data-ttu-id="2a9cf-654">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-654">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-655">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-655">RDBMS</span></span>
* <span data-ttu-id="2a9cf-656">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="2a9cf-656">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-657">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-657">Resource</span></span>
* <span data-ttu-id="2a9cf-658">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-658">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-659">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-659">Role</span></span>
* <span data-ttu-id="2a9cf-660">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="2a9cf-660">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="2a9cf-661">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-661">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="2a9cf-662">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="2a9cf-662">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-663">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-663">Storage</span></span>
* <span data-ttu-id="2a9cf-664">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-664">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-665">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-665">VM</span></span>
* <span data-ttu-id="2a9cf-666">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-666">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="2a9cf-667">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-667">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="2a9cf-668">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="2a9cf-668">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="2a9cf-669">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="2a9cf-669">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="2a9cf-670">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="2a9cf-670">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="2a9cf-671">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-671">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="2a9cf-672">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-672">October 23, 2018</span></span>

<span data-ttu-id="2a9cf-673">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="2a9cf-673">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-674">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-674">Core</span></span>
* <span data-ttu-id="2a9cf-675">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-675">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="2a9cf-676">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-676">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-677">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-677">ACR</span></span>
* <span data-ttu-id="2a9cf-678">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-678">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-679">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-679">CDN</span></span>
* <span data-ttu-id="2a9cf-680">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-680">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="2a9cf-681">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-681">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-682">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-682">Container</span></span>
* <span data-ttu-id="2a9cf-683">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="2a9cf-683">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="2a9cf-684">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-684">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="2a9cf-685">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="2a9cf-685">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="2a9cf-686">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-686">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="2a9cf-687">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="2a9cf-687">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="2a9cf-688">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="2a9cf-688">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="2a9cf-689">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-689">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-690">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-690">CosmosDB</span></span>
* <span data-ttu-id="2a9cf-691">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-691">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-692">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-692">Interactive</span></span>
* <span data-ttu-id="2a9cf-693">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="2a9cf-693">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="2a9cf-694">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2a9cf-694">IoT Central</span></span>
* <span data-ttu-id="2a9cf-695">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="2a9cf-695">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="2a9cf-696">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="2a9cf-696">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-697">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-697">Monitor</span></span>
* <span data-ttu-id="2a9cf-698">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-698">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="2a9cf-699">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-699">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="2a9cf-700">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="2a9cf-700">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="2a9cf-701">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-701">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="2a9cf-702">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-702">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="2a9cf-703">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-703">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="2a9cf-704">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-704">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="2a9cf-705">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="2a9cf-705">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="2a9cf-706">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-706">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="2a9cf-707">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-707">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-708">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-708">Network</span></span>
* <span data-ttu-id="2a9cf-709">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-709">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="2a9cf-710">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-710">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="2a9cf-711">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-711">ServiceBus</span></span>
* <span data-ttu-id="2a9cf-712">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-712">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-713">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-713">SQL</span></span>
* <span data-ttu-id="2a9cf-714">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-714">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-715">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-715">Storage</span></span>
* <span data-ttu-id="2a9cf-716">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-716">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="2a9cf-717">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-717">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-718">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-718">VM</span></span>
* <span data-ttu-id="2a9cf-719">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-719">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="2a9cf-720">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-720">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="2a9cf-721">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-721">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="2a9cf-722">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-722">October 16, 2018</span></span>

<span data-ttu-id="2a9cf-723">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="2a9cf-723">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-724">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-724">VM</span></span>
* <span data-ttu-id="2a9cf-725">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="2a9cf-725">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="2a9cf-726">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-726">October 9, 2018</span></span>

<span data-ttu-id="2a9cf-727">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="2a9cf-727">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-728">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-728">Core</span></span>
* <span data-ttu-id="2a9cf-729">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-729">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-730">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-730">ACR</span></span>
* <span data-ttu-id="2a9cf-731">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="2a9cf-731">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-732">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-732">ACS</span></span>
* <span data-ttu-id="2a9cf-733">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="2a9cf-733">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="2a9cf-734">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="2a9cf-734">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="2a9cf-735">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-735">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="2a9cf-736">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-736">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-737">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-737">Container</span></span>
* <span data-ttu-id="2a9cf-738">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-738">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="2a9cf-739">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-739">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="2a9cf-740">Event Hub</span><span class="sxs-lookup"><span data-stu-id="2a9cf-740">Event Hub</span></span>
* <span data-ttu-id="2a9cf-741">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-741">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="2a9cf-742">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-742">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="2a9cf-743">Extensions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-743">Extensions</span></span>
* <span data-ttu-id="2a9cf-744">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-744">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2a9cf-745">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2a9cf-745">HDInsight</span></span>
* <span data-ttu-id="2a9cf-746">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-746">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-747">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-747">IoT</span></span>
* <span data-ttu-id="2a9cf-748">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="2a9cf-748">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-749">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-749">KeyVault</span></span>
* <span data-ttu-id="2a9cf-750">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="2a9cf-750">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-751">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-751">Network</span></span>
* <span data-ttu-id="2a9cf-752">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-752">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="2a9cf-753">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="2a9cf-753">See #6052</span></span>
* <span data-ttu-id="2a9cf-754">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-754">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="2a9cf-755">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="2a9cf-755">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="2a9cf-756">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-756">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="2a9cf-757">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-757">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="2a9cf-758">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-758">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="2a9cf-759">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-759">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-760">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-760">Role</span></span>
* <span data-ttu-id="2a9cf-761">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-761">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="2a9cf-762">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-762">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="2a9cf-763">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="2a9cf-763">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="2a9cf-764">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-764">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="2a9cf-765">Service Bus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-765">Service Bus</span></span>
* <span data-ttu-id="2a9cf-766">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-766">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-767">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-767">VM</span></span>
* <span data-ttu-id="2a9cf-768">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-768">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="2a9cf-769">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-769">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="2a9cf-770">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-770">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="2a9cf-771">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-771">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="2a9cf-772">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-772">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="2a9cf-773">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-773">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="2a9cf-774">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-774">September 21, 2018</span></span>

<span data-ttu-id="2a9cf-775">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="2a9cf-775">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-776">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-776">ACR</span></span>
* <span data-ttu-id="2a9cf-777">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-777">Added ACR Task commands</span></span>
* <span data-ttu-id="2a9cf-778">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-778">Added quick run command</span></span>
* <span data-ttu-id="2a9cf-779">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-779">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="2a9cf-780">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-780">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="2a9cf-781">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-781">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="2a9cf-782">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="2a9cf-782">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-783">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-783">ACS</span></span>
* <span data-ttu-id="2a9cf-784">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-784">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="2a9cf-785">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="2a9cf-785">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-786">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-786">AppService</span></span>

* <span data-ttu-id="2a9cf-787">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-787">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="2a9cf-788">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="2a9cf-788">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="2a9cf-789">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="2a9cf-789">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="2a9cf-790">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-790">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-791">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-791">Batch</span></span>
* <span data-ttu-id="2a9cf-792">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="2a9cf-792">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="2a9cf-793">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-793">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="2a9cf-794">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-794">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="2a9cf-795">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-795">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2a9cf-796">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-796">Batch AI</span></span> 
* <span data-ttu-id="2a9cf-797">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-797">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2a9cf-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-798">Cognitive Services</span></span>
* <span data-ttu-id="2a9cf-799">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-799">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="2a9cf-800">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-800">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="2a9cf-801">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-801">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="2a9cf-802">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-802">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="2a9cf-803">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-803">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="2a9cf-804">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-804">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-805">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-805">Container</span></span>
* <span data-ttu-id="2a9cf-806">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="2a9cf-806">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="2a9cf-807">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-807">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="2a9cf-808">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-808">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="2a9cf-809">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-809">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="2a9cf-810">DataLake</span><span class="sxs-lookup"><span data-stu-id="2a9cf-810">Datalake</span></span>
* <span data-ttu-id="2a9cf-811">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-811">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="2a9cf-812">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-812">Interactive Shell</span></span>
* <span data-ttu-id="2a9cf-813">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-813">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="2a9cf-814">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-814">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-815">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-815">IoT</span></span>
* <span data-ttu-id="2a9cf-816">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-816">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="2a9cf-817">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-817">Key Vault</span></span>
* <span data-ttu-id="2a9cf-818">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="2a9cf-818">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-819">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-819">Network</span></span>
* <span data-ttu-id="2a9cf-820">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-820">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="2a9cf-821">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-821">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="2a9cf-822">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="2a9cf-822">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="2a9cf-823">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-823">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="2a9cf-824">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-824">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="2a9cf-825">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-825">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="2a9cf-826">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-826">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="2a9cf-827">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-827">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="2a9cf-828">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-828">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="2a9cf-829">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-829">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="2a9cf-830">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-830">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="2a9cf-831">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-831">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="2a9cf-832">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-832">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="2a9cf-833">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-833">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="2a9cf-834">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-834">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="2a9cf-835">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="2a9cf-835">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="2a9cf-836">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-836">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="2a9cf-837">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-837">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-838">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-838">RDBMS</span></span>
* <span data-ttu-id="2a9cf-839">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-839">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="2a9cf-840">Réservation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-840">Reservation</span></span>
* <span data-ttu-id="2a9cf-841">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-841">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="2a9cf-842">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-842">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="2a9cf-843">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="2a9cf-843">Manage App</span></span>
* <span data-ttu-id="2a9cf-844">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-844">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="2a9cf-845">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="2a9cf-845">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-846">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-846">Role</span></span>
* <span data-ttu-id="2a9cf-847">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-847">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="2a9cf-848">SignalR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-848">SignalR</span></span>
* <span data-ttu-id="2a9cf-849">Première version</span><span class="sxs-lookup"><span data-stu-id="2a9cf-849">First release</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-850">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-850">Storage</span></span>
* <span data-ttu-id="2a9cf-851">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="2a9cf-851">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="2a9cf-852">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="2a9cf-852">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-853">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-853">VM</span></span>
* <span data-ttu-id="2a9cf-854">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-854">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="2a9cf-855">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-855">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="2a9cf-856">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-856">August 28, 2018</span></span>

<span data-ttu-id="2a9cf-857">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="2a9cf-857">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-858">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-858">Core</span></span>

* <span data-ttu-id="2a9cf-859">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-859">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="2a9cf-860">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2a9cf-860">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-861">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-861">ACR</span></span>

* <span data-ttu-id="2a9cf-862">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="2a9cf-862">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="2a9cf-863">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-863">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-864">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-864">ACS</span></span>

* <span data-ttu-id="2a9cf-865">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-865">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="2a9cf-866">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="2a9cf-866">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-867">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-867">AppService</span></span>

* <span data-ttu-id="2a9cf-868">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="2a9cf-868">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="2a9cf-869">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="2a9cf-869">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="2a9cf-870">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-870">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="2a9cf-871">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="2a9cf-871">Backup</span></span>

* <span data-ttu-id="2a9cf-872">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-872">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="2a9cf-873">Service de robot</span><span class="sxs-lookup"><span data-stu-id="2a9cf-873">Bot Service</span></span>

* <span data-ttu-id="2a9cf-874">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-874">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2a9cf-875">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-875">Cognitive Services</span></span>

* <span data-ttu-id="2a9cf-876">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-876">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-877">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-877">IoT</span></span>

* <span data-ttu-id="2a9cf-878">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-878">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-879">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-879">Monitor</span></span>

* <span data-ttu-id="2a9cf-880">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-880">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="2a9cf-881">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-881">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-882">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-882">Network</span></span>

* <span data-ttu-id="2a9cf-883">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-883">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-884">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-884">Resource</span></span>

* <span data-ttu-id="2a9cf-885">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-885">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-886">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-886">Storage</span></span>

* <span data-ttu-id="2a9cf-887">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-887">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-888">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-888">VM</span></span>

* <span data-ttu-id="2a9cf-889">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-889">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="2a9cf-890">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-890">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="2a9cf-891">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-891">Auguest 14, 2018</span></span>

<span data-ttu-id="2a9cf-892">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="2a9cf-892">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-893">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-893">Core</span></span>

* <span data-ttu-id="2a9cf-894">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-894">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="2a9cf-895">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="2a9cf-895">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="2a9cf-896">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-896">Telemetry</span></span>

* <span data-ttu-id="2a9cf-897">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-897">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-898">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-898">ACR</span></span>

* <span data-ttu-id="2a9cf-899">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-899">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="2a9cf-900">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-900">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-901">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-901">ACS</span></span>

* <span data-ttu-id="2a9cf-902">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-902">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="2a9cf-903">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-903">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="2a9cf-904">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-904">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="2a9cf-905">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-905">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="2a9cf-906">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="2a9cf-906">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="2a9cf-907">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-907">AppService</span></span>

* <span data-ttu-id="2a9cf-908">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-908">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="2a9cf-909">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="2a9cf-909">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="2a9cf-910">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-910">BatchAI</span></span>

* <span data-ttu-id="2a9cf-911">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="2a9cf-911">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="2a9cf-912">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-912">Container</span></span>

* <span data-ttu-id="2a9cf-913">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-913">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="2a9cf-914">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-914">IoT</span></span>

* <span data-ttu-id="2a9cf-915">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="2a9cf-915">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="2a9cf-916">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-916">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="2a9cf-917">Iot Central</span><span class="sxs-lookup"><span data-stu-id="2a9cf-917">Iot Central</span></span>

* <span data-ttu-id="2a9cf-918">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="2a9cf-918">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-919">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-919">KeyVault</span></span>


* <span data-ttu-id="2a9cf-920">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-920">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="2a9cf-921">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-921">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="2a9cf-922">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="2a9cf-922">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="2a9cf-923">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-923">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="2a9cf-924">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-924">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="2a9cf-925">Relais</span><span class="sxs-lookup"><span data-stu-id="2a9cf-925">Relay</span></span>

* <span data-ttu-id="2a9cf-926">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-926">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-927">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-927">Sql</span></span>

* <span data-ttu-id="2a9cf-928">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-928">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-929">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-929">Storage</span></span>

* <span data-ttu-id="2a9cf-930">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="2a9cf-930">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="2a9cf-931">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-931">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="2a9cf-932">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-932">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="2a9cf-933">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="2a9cf-933">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="2a9cf-934">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-934">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-935">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-935">VM</span></span>

* <span data-ttu-id="2a9cf-936">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-936">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="2a9cf-937">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-937">July 31, 2018</span></span>

<span data-ttu-id="2a9cf-938">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="2a9cf-938">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-939">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-939">ACR</span></span>

* <span data-ttu-id="2a9cf-940">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-940">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="2a9cf-941">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-941">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-942">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-942">ACS</span></span>

* <span data-ttu-id="2a9cf-943">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-943">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-944">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-944">Batch</span></span>

* <span data-ttu-id="2a9cf-945">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="2a9cf-945">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-946">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-946">Container</span></span>

* <span data-ttu-id="2a9cf-947">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="2a9cf-947">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-948">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-948">Network</span></span>

* <span data-ttu-id="2a9cf-949">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2a9cf-949">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="2a9cf-950">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-950">Resource</span></span>

* <span data-ttu-id="2a9cf-951">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-951">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="2a9cf-952">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-952">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-953">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-953">Role</span></span>

* <span data-ttu-id="2a9cf-954">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-954">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="2a9cf-955">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-955">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="2a9cf-956">Recherche</span><span class="sxs-lookup"><span data-stu-id="2a9cf-956">Search</span></span>

* <span data-ttu-id="2a9cf-957">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="2a9cf-957">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="2a9cf-958">Service Bus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-958">Service Bus</span></span>

* <span data-ttu-id="2a9cf-959">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="2a9cf-959">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="2a9cf-960">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-960">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="2a9cf-961">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-961">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="2a9cf-962">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-962">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-963">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-963">Storage</span></span>

* <span data-ttu-id="2a9cf-964">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-964">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="2a9cf-965">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-965">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-966">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-966">VM</span></span>

* <span data-ttu-id="2a9cf-967">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-967">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="2a9cf-968">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-968">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="2a9cf-969">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="2a9cf-969">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="2a9cf-970">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-970">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="2a9cf-971">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-971">July 18, 2018</span></span>

<span data-ttu-id="2a9cf-972">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="2a9cf-972">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-973">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-973">Core</span></span>

* <span data-ttu-id="2a9cf-974">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-974">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="2a9cf-975">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-975">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="2a9cf-976">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-976">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-977">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-977">ACR</span></span>

* <span data-ttu-id="2a9cf-978">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-978">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="2a9cf-979">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-979">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="2a9cf-980">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-980">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="2a9cf-981">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-981">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-982">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-982">ACS</span></span>

* <span data-ttu-id="2a9cf-983">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="2a9cf-983">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-984">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-984">AppService</span></span>

* <span data-ttu-id="2a9cf-985">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-985">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-986">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-986">Batch</span></span>

* <span data-ttu-id="2a9cf-987">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="2a9cf-987">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="2a9cf-988">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-988">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2a9cf-989">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-989">Batch AI</span></span>

* <span data-ttu-id="2a9cf-990">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-990">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-991">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-991">Container</span></span>

* <span data-ttu-id="2a9cf-992">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="2a9cf-992">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="2a9cf-993">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="2a9cf-993">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-994">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-994">Network</span></span>

* <span data-ttu-id="2a9cf-995">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-995">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="2a9cf-996">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-996">Added `network nic wait`</span></span>
* <span data-ttu-id="2a9cf-997">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-997">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="2a9cf-998">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-998">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="2a9cf-999">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-999">Resource</span></span>

* <span data-ttu-id="2a9cf-1000">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1000">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="2a9cf-1001">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1001">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="2a9cf-1002">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1002">Added `deployment wait` command</span></span>
* <span data-ttu-id="2a9cf-1003">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1003">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1004">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1004">SQL</span></span>

* <span data-ttu-id="2a9cf-1005">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1005">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="2a9cf-1006">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1006">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="2a9cf-1007">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1007">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1008">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1008">Storage</span></span>

* <span data-ttu-id="2a9cf-1009">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1009">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1010">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1010">VM</span></span>

* <span data-ttu-id="2a9cf-1011">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1011">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="2a9cf-1012">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1012">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="2a9cf-1013">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1013">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="2a9cf-1014">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1014">July 3, 2018</span></span>

<span data-ttu-id="2a9cf-1015">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1015">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="2a9cf-1016">AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1016">AKS</span></span>

* <span data-ttu-id="2a9cf-1017">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1017">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="2a9cf-1018">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1018">July 3, 2018</span></span>

<span data-ttu-id="2a9cf-1019">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1019">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1020">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1020">Core</span></span>

* <span data-ttu-id="2a9cf-1021">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1021">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1022">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1022">ACR</span></span>

* <span data-ttu-id="2a9cf-1023">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1023">Added polling build status</span></span>
* <span data-ttu-id="2a9cf-1024">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1024">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="2a9cf-1025">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1025">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1026">ACS</span></span>

* <span data-ttu-id="2a9cf-1027">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1027">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="2a9cf-1028">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1028">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="2a9cf-1029">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1029">Updated options for `aks browse` command.</span></span> <span data-ttu-id="2a9cf-1030">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1030">Added `--listen-port` support</span></span>
* <span data-ttu-id="2a9cf-1031">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1031">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="2a9cf-1032">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1032">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="2a9cf-1033">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1033">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1034">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1034">AppService</span></span>

* <span data-ttu-id="2a9cf-1035">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1035">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="2a9cf-1036">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1036">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="2a9cf-1037">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1037">Backup</span></span>

* <span data-ttu-id="2a9cf-1038">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1038">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="2a9cf-1039">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1039">BatchAI</span></span>

* <span data-ttu-id="2a9cf-1040">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1040">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="2a9cf-1041">Cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1041">Cloud</span></span>

* <span data-ttu-id="2a9cf-1042">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1042">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1043">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1043">Container</span></span>

* <span data-ttu-id="2a9cf-1044">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1044">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="2a9cf-1045">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1045">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="2a9cf-1046">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1046">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1047">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1047">Extension</span></span>

* <span data-ttu-id="2a9cf-1048">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1048">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1049">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1049">Network</span></span>

* <span data-ttu-id="2a9cf-1050">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1050">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-1051">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1051">Rdbms</span></span>

* <span data-ttu-id="2a9cf-1052">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1052">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1053">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1053">Resource</span></span>

* <span data-ttu-id="2a9cf-1054">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1054">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1055">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1055">VM</span></span>

* <span data-ttu-id="2a9cf-1056">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1056">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="2a9cf-1057">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1057">June 25, 2018</span></span>

<span data-ttu-id="2a9cf-1058">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1058">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="2a9cf-1059">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1059">CLI</span></span>

* <span data-ttu-id="2a9cf-1060">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1060">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="2a9cf-1061">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1061">June 19, 2018</span></span>

<span data-ttu-id="2a9cf-1062">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1062">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1063">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1063">Core</span></span>

* <span data-ttu-id="2a9cf-1064">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1064">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1065">ACR</span></span>

* <span data-ttu-id="2a9cf-1066">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1066">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="2a9cf-1067">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1067">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1068">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1068">ACS</span></span>

* <span data-ttu-id="2a9cf-1069">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1069">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="2a9cf-1070">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1070">Added `--update` support</span></span>
* <span data-ttu-id="2a9cf-1071">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1071">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="2a9cf-1072">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1072">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="2a9cf-1073">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1073">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="2a9cf-1074">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1074">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="2a9cf-1075">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1075">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="2a9cf-1076">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1076">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1077">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1077">AppService</span></span>

* <span data-ttu-id="2a9cf-1078">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1078">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="2a9cf-1079">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1079">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-1080">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1080">Batch</span></span>

* <span data-ttu-id="2a9cf-1081">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1081">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2a9cf-1082">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1082">Batch AI</span></span>

* <span data-ttu-id="2a9cf-1083">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1083">Added support for workspaces.</span></span> <span data-ttu-id="2a9cf-1084">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1084">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="2a9cf-1085">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1085">Added support for experiments.</span></span> <span data-ttu-id="2a9cf-1086">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1086">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="2a9cf-1087">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1087">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="2a9cf-1088">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1088">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="2a9cf-1089">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1089">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="2a9cf-1090">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1090">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="2a9cf-1091">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1091">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="2a9cf-1092">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1092">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="2a9cf-1093">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1093">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="2a9cf-1094">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1094">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="2a9cf-1095">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1095">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="2a9cf-1096">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1096">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="2a9cf-1097">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1097">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="2a9cf-1098">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1098">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="2a9cf-1099">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1099">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="2a9cf-1100">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1100">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="2a9cf-1101">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1101">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="2a9cf-1102">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1102">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="2a9cf-1103">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1103">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="2a9cf-1104">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1104">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="2a9cf-1105">Cartes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1105">Maps</span></span>

* <span data-ttu-id="2a9cf-1106">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1106">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1107">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1107">Network</span></span>

* <span data-ttu-id="2a9cf-1108">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1108">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="2a9cf-1109">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1109">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="2a9cf-1110">#6502</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1110">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="2a9cf-1111">Réservations</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1111">Reservations</span></span>

* <span data-ttu-id="2a9cf-1112">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1112">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="2a9cf-1113">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1113">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="2a9cf-1114">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1114">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="2a9cf-1115">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1115">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="2a9cf-1116">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1116">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="2a9cf-1117">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1117">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1118">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1118">Role</span></span>

* <span data-ttu-id="2a9cf-1119">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1119">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1120">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1120">SQL</span></span>

* <span data-ttu-id="2a9cf-1121">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1121">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1122">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1122">Storage</span></span>

* <span data-ttu-id="2a9cf-1123">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1123">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1124">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1124">VM</span></span>

* <span data-ttu-id="2a9cf-1125">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1125">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="2a9cf-1126">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1126">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="2a9cf-1127">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1127">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="2a9cf-1128">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1128">June 13, 2018</span></span>

<span data-ttu-id="2a9cf-1129">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1129">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1130">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1130">Core</span></span>

* <span data-ttu-id="2a9cf-1131">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1131">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="2a9cf-1132">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1132">June 13, 2018</span></span>

<span data-ttu-id="2a9cf-1133">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1133">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="2a9cf-1134">AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1134">AKS</span></span>

* <span data-ttu-id="2a9cf-1135">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1135">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="2a9cf-1136">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1136">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="2a9cf-1137">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1137">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="2a9cf-1138">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1138">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="2a9cf-1139">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1139">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1140">AppService</span></span>

* <span data-ttu-id="2a9cf-1141">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1141">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="2a9cf-1142">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1142">June 5, 2018</span></span>

<span data-ttu-id="2a9cf-1143">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1143">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1144">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1144">Interactive</span></span>

* <span data-ttu-id="2a9cf-1145">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1145">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="2a9cf-1146">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1146">June 5, 2018</span></span>

<span data-ttu-id="2a9cf-1147">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1147">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1148">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1148">Core</span></span>

* <span data-ttu-id="2a9cf-1149">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1149">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="2a9cf-1150">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1150">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1151">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1151">ACR</span></span>

* <span data-ttu-id="2a9cf-1152">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1152">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="2a9cf-1153">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1153">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="2a9cf-1154">AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1154">AKS</span></span>

* <span data-ttu-id="2a9cf-1155">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1155">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-1156">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1156">Batch</span></span>

* <span data-ttu-id="2a9cf-1157">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1157">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-1158">IOT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1158">IOT</span></span>

* <span data-ttu-id="2a9cf-1159">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1159">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1160">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1160">Network</span></span>

* <span data-ttu-id="2a9cf-1161">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1161">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="2a9cf-1162">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1162">Policy Insights</span></span>

* <span data-ttu-id="2a9cf-1163">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1163">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="2a9cf-1164">ARM</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1164">ARM</span></span>

* <span data-ttu-id="2a9cf-1165">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1165">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1166">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1166">SQL</span></span>

* <span data-ttu-id="2a9cf-1167">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1167">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="2a9cf-1168">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1168">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="2a9cf-1169">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1169">Storage</span></span>

* <span data-ttu-id="2a9cf-1170">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1170">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1171">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1171">VM</span></span>

* <span data-ttu-id="2a9cf-1172">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1172">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="2a9cf-1173">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1173">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="2a9cf-1174">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1174">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="2a9cf-1175">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1175">May 22, 2018</span></span>

<span data-ttu-id="2a9cf-1176">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1176">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1177">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1177">Core</span></span>

* <span data-ttu-id="2a9cf-1178">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1178">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1179">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1179">ACS</span></span>

* <span data-ttu-id="2a9cf-1180">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1180">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="2a9cf-1181">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1181">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1182">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1182">AppService</span></span>

* <span data-ttu-id="2a9cf-1183">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1183">Improved generic update commands</span></span>
* <span data-ttu-id="2a9cf-1184">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1184">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1185">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1185">Container</span></span>

* <span data-ttu-id="2a9cf-1186">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1186">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="2a9cf-1187">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1187">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1188">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1188">Extension</span></span>

* <span data-ttu-id="2a9cf-1189">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1189">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1190">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1190">Interactive</span></span>

* <span data-ttu-id="2a9cf-1191">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1191">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="2a9cf-1192">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1192">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-1193">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1193">KeyVault</span></span>

* <span data-ttu-id="2a9cf-1194">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1194">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1195">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1195">Network</span></span>

* <span data-ttu-id="2a9cf-1196">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1196">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="2a9cf-1197">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1197">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1198">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1198">SQL</span></span>

* <span data-ttu-id="2a9cf-1199">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1199">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="2a9cf-1200">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1200">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="2a9cf-1201">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1201">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="2a9cf-1202">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1202">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="2a9cf-1203">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1203">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="2a9cf-1204">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1204">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="2a9cf-1205">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1205">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="2a9cf-1206">`edition`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1206">`edition`.</span></span> <span data-ttu-id="2a9cf-1207">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1207">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="2a9cf-1208">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1208">`elasticPoolName`.</span></span> <span data-ttu-id="2a9cf-1209">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1209">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="2a9cf-1210">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1210">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="2a9cf-1211">`edition`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1211">`edition`.</span></span> <span data-ttu-id="2a9cf-1212">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1212">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="2a9cf-1213">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1213">`dtu`.</span></span> <span data-ttu-id="2a9cf-1214">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1214">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="2a9cf-1215">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1215">`databaseDtuMin`.</span></span> <span data-ttu-id="2a9cf-1216">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1216">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="2a9cf-1217">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1217">`databaseDtuMax`.</span></span> <span data-ttu-id="2a9cf-1218">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1218">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="2a9cf-1219">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1219">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="2a9cf-1220">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1220">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1221">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1221">Storage</span></span>

* <span data-ttu-id="2a9cf-1222">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1222">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="2a9cf-1223">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1223">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1224">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1224">VM</span></span>

* <span data-ttu-id="2a9cf-1225">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1225">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="2a9cf-1226">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1226">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="2a9cf-1227">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1227">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="2a9cf-1228">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1228">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="2a9cf-1229">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1229">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="2a9cf-1230">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1230">May 7, 2018</span></span>

<span data-ttu-id="2a9cf-1231">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1231">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1232">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1232">Core</span></span>

* <span data-ttu-id="2a9cf-1233">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1233">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="2a9cf-1234">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1234">Added limited support for positional arguments</span></span>
* <span data-ttu-id="2a9cf-1235">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1235">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="2a9cf-1236">#5591</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1236">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="2a9cf-1237">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1237">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="2a9cf-1238">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1238">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="2a9cf-1239">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1239">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="2a9cf-1240">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1240">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="2a9cf-1241">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1241">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1242">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1242">ACR</span></span>

* <span data-ttu-id="2a9cf-1243">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1243">Added ACR Build commands</span></span>
* <span data-ttu-id="2a9cf-1244">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1244">Improved resource not found error messages</span></span>
* <span data-ttu-id="2a9cf-1245">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1245">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="2a9cf-1246">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1246">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="2a9cf-1247">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1247">Improved repository commands error messages</span></span>
* <span data-ttu-id="2a9cf-1248">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1248">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1249">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1249">ACS</span></span>

* <span data-ttu-id="2a9cf-1250">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1250">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="2a9cf-1251">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1251">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="2a9cf-1252">AMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1252">AMS</span></span>

* <span data-ttu-id="2a9cf-1253">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1253">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1254">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1254">Appservice</span></span>

* <span data-ttu-id="2a9cf-1255">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1255">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="2a9cf-1256">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1256">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="2a9cf-1257">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1257">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="2a9cf-1258">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1258">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2a9cf-1259">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1259">Batch AI</span></span>

* <span data-ttu-id="2a9cf-1260">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1260">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2a9cf-1261">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1261">Cognitive Services</span></span>

* <span data-ttu-id="2a9cf-1262">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1262">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-1263">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1263">Consumption</span></span>

* <span data-ttu-id="2a9cf-1264">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1264">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1265">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1265">Container</span></span>

* <span data-ttu-id="2a9cf-1266">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1266">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2a9cf-1267">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1267">Cosmos DB</span></span>

* <span data-ttu-id="2a9cf-1268">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1268">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="2a9cf-1269">DMS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1269">DMS</span></span>

* <span data-ttu-id="2a9cf-1270">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1270">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1271">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1271">Extension</span></span>

* <span data-ttu-id="2a9cf-1272">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1272">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1273">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1273">Interactive</span></span>

* <span data-ttu-id="2a9cf-1274">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1274">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="2a9cf-1275">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1275">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="2a9cf-1276">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1276">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="2a9cf-1277">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1277">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="2a9cf-1278">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1278">Lab</span></span>

* <span data-ttu-id="2a9cf-1279">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1279">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1280">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1280">Network</span></span>

* <span data-ttu-id="2a9cf-1281">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1281">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="2a9cf-1282">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1282">Profile</span></span>

* <span data-ttu-id="2a9cf-1283">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1283">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="2a9cf-1284">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1284">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="2a9cf-1285">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1285">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="2a9cf-1286">Redis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1286">Redis</span></span>

* <span data-ttu-id="2a9cf-1287">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1287">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="2a9cf-1288">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1288">Deprecated `redis list-all`.</span></span> <span data-ttu-id="2a9cf-1289">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1289">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="2a9cf-1290">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1290">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="2a9cf-1291">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1291">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1292">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1292">Role</span></span>

* <span data-ttu-id="2a9cf-1293">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1293">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1294">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1294">Storage</span></span>

* <span data-ttu-id="2a9cf-1295">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1295">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="2a9cf-1296">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1296">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="2a9cf-1297">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1297">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="2a9cf-1298">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1298">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="2a9cf-1299">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1299">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1300">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1300">VM</span></span>

* <span data-ttu-id="2a9cf-1301">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1301">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="2a9cf-1302">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1302">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="2a9cf-1303">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1303">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="2a9cf-1304">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1304">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="2a9cf-1305">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1305">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="2a9cf-1306">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1306">Added write accelerator support</span></span>
* <span data-ttu-id="2a9cf-1307">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1307">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="2a9cf-1308">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1308">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="2a9cf-1309">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1309">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="2a9cf-1310">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1310">April 10, 2018</span></span>

<span data-ttu-id="2a9cf-1311">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1311">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1312">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1312">ACR</span></span>

* <span data-ttu-id="2a9cf-1313">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1313">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1314">ACS</span></span>

* <span data-ttu-id="2a9cf-1315">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1315">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1316">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1316">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="2a9cf-1318">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1318">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="2a9cf-1319">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1319">BatchAI</span></span>

* <span data-ttu-id="2a9cf-1320">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1320">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="2a9cf-1321">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1321">Job level mounting</span></span>
  - <span data-ttu-id="2a9cf-1322">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1322">Environment variables with secret values</span></span>
  - <span data-ttu-id="2a9cf-1323">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1323">Performance counters settings</span></span>
  - <span data-ttu-id="2a9cf-1324">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1324">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="2a9cf-1325">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1325">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="2a9cf-1326">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1326">Usage and limits reporting</span></span>
  - <span data-ttu-id="2a9cf-1327">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1327">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="2a9cf-1328">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1328">Support for custom images</span></span>
  - <span data-ttu-id="2a9cf-1329">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1329">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="2a9cf-1330">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1330">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="2a9cf-1331">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1331">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="2a9cf-1332">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1332">National clouds are supported</span></span>
* <span data-ttu-id="2a9cf-1333">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1333">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="2a9cf-1334">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1334">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="2a9cf-1335">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1335">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="2a9cf-1336">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1336">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="2a9cf-1337">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1337">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="2a9cf-1338">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1338">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="2a9cf-1339">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1339">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="2a9cf-1340">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1340">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="2a9cf-1341">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1341">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="2a9cf-1342">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1342">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="2a9cf-1343">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1343">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="2a9cf-1344">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1344">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="2a9cf-1345">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1345">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="2a9cf-1346">Facturation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1346">Billing</span></span>

* <span data-ttu-id="2a9cf-1347">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1347">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-1348">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1348">Consumption</span></span>

* <span data-ttu-id="2a9cf-1349">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1349">Added `marketplace` commands</span></span>
* <span data-ttu-id="2a9cf-1350">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1350">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="2a9cf-1351">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1351">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="2a9cf-1352">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1352">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="2a9cf-1353">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1353">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="2a9cf-1354">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1354">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1355">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1355">Container</span></span>

* <span data-ttu-id="2a9cf-1356">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1356">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="2a9cf-1357">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1357">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1358">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1358">Extension</span></span>

* <span data-ttu-id="2a9cf-1359">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1359">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1360">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1360">Interactive</span></span>

* <span data-ttu-id="2a9cf-1361">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1361">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="2a9cf-1362">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1362">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="2a9cf-1363">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1363">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1364">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1364">Network</span></span>

* <span data-ttu-id="2a9cf-1365">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1365">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="2a9cf-1366">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1366">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="2a9cf-1367">#4910</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1367">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="2a9cf-1368">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1368">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="2a9cf-1369">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1369">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="2a9cf-1370">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1370">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1371">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1371">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1372">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1372">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1373">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1373">Profile</span></span>

* <span data-ttu-id="2a9cf-1374">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1374">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="2a9cf-1375">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1375">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-1376">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1376">RDBMS</span></span>

* <span data-ttu-id="2a9cf-1377">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1377">Added `georestore` command</span></span>
* <span data-ttu-id="2a9cf-1378">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1378">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1379">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1379">Resource</span></span>

* <span data-ttu-id="2a9cf-1380">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1380">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="2a9cf-1381">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1381">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1382">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1382">SQL</span></span>

* <span data-ttu-id="2a9cf-1383">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1383">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1384">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1384">Storage</span></span>

* <span data-ttu-id="2a9cf-1385">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1385">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1386">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1386">VM</span></span>

* <span data-ttu-id="2a9cf-1387">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1387">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="2a9cf-1388">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1388">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="2a9cf-1390">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1390">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="2a9cf-1391">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1391">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="2a9cf-1392">#5718</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1392">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="2a9cf-1393">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1393">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="2a9cf-1394">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1394">March 27, 2018</span></span>

<span data-ttu-id="2a9cf-1395">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1395">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1396">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1396">Core</span></span>

* <span data-ttu-id="2a9cf-1397">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1397">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1398">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1398">ACS</span></span>

* <span data-ttu-id="2a9cf-1399">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1399">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1400">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1400">Appservice</span></span>

* <span data-ttu-id="2a9cf-1401">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1401">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="2a9cf-1402">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1402">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="2a9cf-1403">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1403">Backup</span></span>

* <span data-ttu-id="2a9cf-1404">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1404">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="2a9cf-1405">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1405">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="2a9cf-1406">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1406">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="2a9cf-1407">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1407">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1408">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1408">Container</span></span>

* <span data-ttu-id="2a9cf-1409">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1409">Added `container exec` command.</span></span> <span data-ttu-id="2a9cf-1410">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1410">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="2a9cf-1411">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1411">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1412">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1412">Extension</span></span>

* <span data-ttu-id="2a9cf-1413">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1413">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="2a9cf-1414">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1414">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="2a9cf-1415">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1415">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1416">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1416">Interactive</span></span>

* <span data-ttu-id="2a9cf-1417">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1417">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="2a9cf-1418">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1418">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="2a9cf-1419">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1419">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="2a9cf-1420">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1420">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="2a9cf-1421">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1421">Lab</span></span>

* <span data-ttu-id="2a9cf-1422">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1422">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1423">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1423">Monitor</span></span>

* <span data-ttu-id="2a9cf-1424">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1424">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="2a9cf-1425">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1425">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="2a9cf-1426">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1426">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1427">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1427">Network</span></span>

* <span data-ttu-id="2a9cf-1428">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1428">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1429">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1429">Profile</span></span>

* <span data-ttu-id="2a9cf-1430">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1430">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-1431">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1431">RDBMS</span></span>

* <span data-ttu-id="2a9cf-1432">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1432">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1433">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1433">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="2a9cf-1435">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1435">Role</span></span>

* <span data-ttu-id="2a9cf-1436">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1436">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="2a9cf-1437">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1437">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="2a9cf-1438">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1438">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="2a9cf-1439">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1439">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="2a9cf-1440">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1440">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1441">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1441">Storage</span></span>

* <span data-ttu-id="2a9cf-1442">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1442">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="2a9cf-1443">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1443">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1444">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1444">VM</span></span>

* <span data-ttu-id="2a9cf-1445">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1445">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="2a9cf-1446">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1446">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="2a9cf-1447">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1447">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="2a9cf-1448">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1448">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="2a9cf-1449">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1449">March 13, 2018</span></span>

<span data-ttu-id="2a9cf-1450">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1450">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1451">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1451">ACR</span></span>

* <span data-ttu-id="2a9cf-1452">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1452">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="2a9cf-1453">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1453">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="2a9cf-1454">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1454">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1455">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1455">ACS</span></span>

* <span data-ttu-id="2a9cf-1456">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1456">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="2a9cf-1457">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1457">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="2a9cf-1458">Advisor</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1458">Advisor</span></span>

* <span data-ttu-id="2a9cf-1459">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1459">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="2a9cf-1460">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1460">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="2a9cf-1461">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1461">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="2a9cf-1462">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1462">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="2a9cf-1463">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1463">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1464">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1464">Appservice</span></span>

* <span data-ttu-id="2a9cf-1465">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1465">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="2a9cf-1466">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1466">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="2a9cf-1467">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1467">Eventhubs</span></span>

* <span data-ttu-id="2a9cf-1468">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1468">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1469">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1469">Extension</span></span>

* <span data-ttu-id="2a9cf-1470">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1470">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1471">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1471">Interactive</span></span>

* <span data-ttu-id="2a9cf-1472">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1472">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="2a9cf-1473">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1473">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="2a9cf-1474">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1474">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="2a9cf-1475">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1475">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1476">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1476">Monitor</span></span>

* <span data-ttu-id="2a9cf-1477">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1477">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="2a9cf-1478">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1478">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="2a9cf-1479">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1479">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="2a9cf-1480">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1480">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1481">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1481">Network</span></span>

* <span data-ttu-id="2a9cf-1482">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1482">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="2a9cf-1483">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1483">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="2a9cf-1484">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1484">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="2a9cf-1485">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1485">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1486">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1486">Profile</span></span>

* <span data-ttu-id="2a9cf-1487">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1487">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="2a9cf-1488">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1488">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-1489">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1489">RDBMS</span></span>

* <span data-ttu-id="2a9cf-1490">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1490">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="2a9cf-1491">Service Bus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1491">Service Bus</span></span>

* <span data-ttu-id="2a9cf-1492">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1492">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1493">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1493">Storage</span></span>

* <span data-ttu-id="2a9cf-1494">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1494">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="2a9cf-1495">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1495">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1496">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1496">VM</span></span>

* <span data-ttu-id="2a9cf-1497">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1497">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="2a9cf-1498">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1498">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="2a9cf-1499">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1499">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="2a9cf-1500">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1500">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="2a9cf-1501">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1501">February 27, 2018</span></span>

<span data-ttu-id="2a9cf-1502">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1502">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1503">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1503">Core</span></span>

* <span data-ttu-id="2a9cf-1504">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1504">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="2a9cf-1505">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1505">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="2a9cf-1506">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1506">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1507">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1507">ACS</span></span>

* <span data-ttu-id="2a9cf-1508">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1508">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="2a9cf-1509">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1509">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="2a9cf-1510">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1510">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="2a9cf-1511">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1511">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1512">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1512">Appservice</span></span>

* <span data-ttu-id="2a9cf-1513">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1513">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="2a9cf-1514">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1514">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2a9cf-1515">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1515">Cognitive Services</span></span>

* <span data-ttu-id="2a9cf-1516">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1516">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-1517">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1517">Consumption</span></span>

* <span data-ttu-id="2a9cf-1518">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1518">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="2a9cf-1519">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1519">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1520">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1520">Container</span></span>

* <span data-ttu-id="2a9cf-1521">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1521">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1522">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1522">Network</span></span>

* <span data-ttu-id="2a9cf-1523">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1523">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1524">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1524">Resource</span></span>

* <span data-ttu-id="2a9cf-1525">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1525">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1526">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1526">Role</span></span>

* <span data-ttu-id="2a9cf-1527">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1527">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1528">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1528">SQL</span></span>

* <span data-ttu-id="2a9cf-1529">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1529">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1530">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1530">Storage</span></span>

* <span data-ttu-id="2a9cf-1531">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1531">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1532">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1532">VM</span></span>

* <span data-ttu-id="2a9cf-1533">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1533">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="2a9cf-1534">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1534">February 13, 2018</span></span>

<span data-ttu-id="2a9cf-1535">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1535">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1536">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1536">Core</span></span>

* <span data-ttu-id="2a9cf-1537">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1537">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1538">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1538">ACS</span></span>

* <span data-ttu-id="2a9cf-1539">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1539">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="2a9cf-1540">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1540">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="2a9cf-1541">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1541">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="2a9cf-1542">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1542">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="2a9cf-1543">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1543">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="2a9cf-1544">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1544">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="2a9cf-1545">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1545">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="2a9cf-1546">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1546">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1547">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1547">Appservice</span></span>

* <span data-ttu-id="2a9cf-1548">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1548">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="2a9cf-1549">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1549">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1550">CDN</span></span>

* <span data-ttu-id="2a9cf-1551">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1551">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1552">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1552">Container</span></span>

* <span data-ttu-id="2a9cf-1553">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1553">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="2a9cf-1554">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1554">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-1555">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1555">CosmosDB</span></span>

* <span data-ttu-id="2a9cf-1556">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1556">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1557">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1557">Extension</span></span>

* <span data-ttu-id="2a9cf-1558">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1558">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="2a9cf-1559">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1559">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="2a9cf-1560">Commentaires</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1560">Feedback</span></span>

* <span data-ttu-id="2a9cf-1561">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1561">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1562">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1562">Interactive</span></span>

* <span data-ttu-id="2a9cf-1563">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1563">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="2a9cf-1564">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1564">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1565">IoT</span></span>

* <span data-ttu-id="2a9cf-1566">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1566">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="2a9cf-1567">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1567">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="2a9cf-1568">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1568">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1569">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1569">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1570">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1570">Monitor</span></span>

* <span data-ttu-id="2a9cf-1571">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1571">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1572">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1572">Network</span></span>

* <span data-ttu-id="2a9cf-1573">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1573">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="2a9cf-1574">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1574">Profile</span></span>

* <span data-ttu-id="2a9cf-1575">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1575">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1576">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1576">Resource</span></span>

* <span data-ttu-id="2a9cf-1577">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1577">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1578">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1578">Role</span></span>

* <span data-ttu-id="2a9cf-1579">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1579">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1580">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1580">SQL</span></span>

* <span data-ttu-id="2a9cf-1581">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1581">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="2a9cf-1582">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1582">Added `sql db rename`</span></span>
* <span data-ttu-id="2a9cf-1583">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1583">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1584">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1584">Storage</span></span>

* <span data-ttu-id="2a9cf-1585">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1585">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1586">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1586">VM</span></span>

* <span data-ttu-id="2a9cf-1587">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1587">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="2a9cf-1588">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1588">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="2a9cf-1589">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1589">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="2a9cf-1590">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1590">January 31, 2018</span></span>

<span data-ttu-id="2a9cf-1591">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1591">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1592">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1592">Core</span></span>

* <span data-ttu-id="2a9cf-1593">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1593">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="2a9cf-1594">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1594">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="2a9cf-1595">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1595">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="2a9cf-1596">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1596">Use `--verbose` to see</span></span>
* <span data-ttu-id="2a9cf-1597">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1597">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1598">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1598">ACS</span></span>

* <span data-ttu-id="2a9cf-1599">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1599">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="2a9cf-1600">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1600">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1601">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1601">Appservice</span></span>

* <span data-ttu-id="2a9cf-1602">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1602">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="2a9cf-1603">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1603">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-1604">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1604">CDN</span></span>

* <span data-ttu-id="2a9cf-1605">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1605">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-1606">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1606">CosmosDB</span></span>

* <span data-ttu-id="2a9cf-1607">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1607">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1608">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1608">Interactive</span></span>

* <span data-ttu-id="2a9cf-1609">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1609">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1610">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1610">Network</span></span>

* <span data-ttu-id="2a9cf-1611">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1611">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="2a9cf-1612">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1612">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="2a9cf-1613">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1613">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="2a9cf-1614">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1614">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="2a9cf-1615">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1615">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="2a9cf-1616">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1616">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="2a9cf-1617">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1617">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="2a9cf-1618">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1618">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="2a9cf-1619">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1619">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="2a9cf-1620">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1620">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1621">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1621">Profile</span></span>

* <span data-ttu-id="2a9cf-1622">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1622">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1623">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1623">Resource</span></span>

* <span data-ttu-id="2a9cf-1624">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1624">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1625">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1625">Storage</span></span>

* <span data-ttu-id="2a9cf-1626">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1626">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="2a9cf-1627">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1627">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="2a9cf-1628">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1628">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="2a9cf-1629">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1629">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="2a9cf-1630">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1630">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1631">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1631">VM</span></span>

* <span data-ttu-id="2a9cf-1632">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1632">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="2a9cf-1633">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1633">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="2a9cf-1634">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1634">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="2a9cf-1635">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1635">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="2a9cf-1636">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1636">January 17, 2018</span></span>

<span data-ttu-id="2a9cf-1637">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1637">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1638">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1638">ACR</span></span>

* <span data-ttu-id="2a9cf-1639">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1639">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="2a9cf-1640">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1640">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1641">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1641">ACS</span></span>

* <span data-ttu-id="2a9cf-1642">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1642">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="2a9cf-1643">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1643">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1644">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1644">Appservice</span></span>

* <span data-ttu-id="2a9cf-1645">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1645">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="2a9cf-1646">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1646">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="2a9cf-1647">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1647">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="2a9cf-1648">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1648">Backup</span></span>

* <span data-ttu-id="2a9cf-1649">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1649">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="2a9cf-1650">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1650">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="2a9cf-1651">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1651">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="2a9cf-1652">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1652">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="2a9cf-1653">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1653">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-1654">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1654">Batch</span></span>

* <span data-ttu-id="2a9cf-1655">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1655">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="2a9cf-1656">Cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1656">Cloud</span></span>

* <span data-ttu-id="2a9cf-1657">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1657">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-1658">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1658">Consumption</span></span>

* <span data-ttu-id="2a9cf-1659">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1659">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="2a9cf-1660">Event Grid</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1660">Event Grid</span></span>

* <span data-ttu-id="2a9cf-1661">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1661">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="2a9cf-1662">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1662">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="2a9cf-1663">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1663">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="2a9cf-1664">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1664">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="2a9cf-1665">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1665">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="2a9cf-1666">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1666">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="2a9cf-1667">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1667">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="2a9cf-1668">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1668">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-1669">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1669">Interactive</span></span>

* <span data-ttu-id="2a9cf-1670">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1670">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="2a9cf-1671">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1671">Fixed errors on startup</span></span>
* <span data-ttu-id="2a9cf-1672">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1672">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-1673">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1673">IoT</span></span>

* <span data-ttu-id="2a9cf-1674">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1674">Added support for device provisioning service</span></span>
* <span data-ttu-id="2a9cf-1675">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1675">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="2a9cf-1676">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1676">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1677">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1677">Monitor</span></span>

* <span data-ttu-id="2a9cf-1678">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1678">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="2a9cf-1679">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1679">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="2a9cf-1680">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1680">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1681">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1681">Network</span></span>

* <span data-ttu-id="2a9cf-1682">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1682">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="2a9cf-1683">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1683">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1684">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1684">Profile</span></span>

* <span data-ttu-id="2a9cf-1685">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1685">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1686">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1686">Role</span></span>

* <span data-ttu-id="2a9cf-1687">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1687">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2a9cf-1688">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1688">Service Fabric</span></span>

* <span data-ttu-id="2a9cf-1689">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1689">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="2a9cf-1690">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1690">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1691">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1691">VM</span></span>

* <span data-ttu-id="2a9cf-1692">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1692">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="2a9cf-1693">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1693">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="2a9cf-1694">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1694">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="2a9cf-1695">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1695">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="2a9cf-1696">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1696">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="2a9cf-1697">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1697">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="2a9cf-1698">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1698">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="2a9cf-1699">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1699">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="2a9cf-1700">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1700">December 19, 2017</span></span>

<span data-ttu-id="2a9cf-1701">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1701">Version 2.0.23</span></span>

* <span data-ttu-id="2a9cf-1702">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1702">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1703">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1703">Container</span></span>

* <span data-ttu-id="2a9cf-1704">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1704">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1705">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1705">Network</span></span>

* <span data-ttu-id="2a9cf-1706">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1706">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1707">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1707">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1708">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1708">Storage</span></span>

* <span data-ttu-id="2a9cf-1709">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1709">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1710">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1710">VM</span></span>

* <span data-ttu-id="2a9cf-1711">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1711">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="2a9cf-1712">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1712">December 5, 2017</span></span>

<span data-ttu-id="2a9cf-1713">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1713">Version 2.0.22</span></span>

* <span data-ttu-id="2a9cf-1714">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1714">Removed `az component` commands.</span></span> <span data-ttu-id="2a9cf-1715">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1715">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1716">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1716">Core</span></span>
* <span data-ttu-id="2a9cf-1717">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1717">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="2a9cf-1718">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1718">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1719">ACS</span></span>

* <span data-ttu-id="2a9cf-1720">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1720">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="2a9cf-1721">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1721">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="2a9cf-1722">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1722">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="2a9cf-1723">Advisor</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1723">Advisor</span></span>

* <span data-ttu-id="2a9cf-1724">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1724">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1725">Appservice</span></span>

* <span data-ttu-id="2a9cf-1726">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1726">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="2a9cf-1727">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1727">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="2a9cf-1728">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1728">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="2a9cf-1729">Consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1729">Consumption</span></span>

* <span data-ttu-id="2a9cf-1730">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1730">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1731">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1731">Container</span></span>

* <span data-ttu-id="2a9cf-1732">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1732">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1733">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1733">Monitor</span></span>

* <span data-ttu-id="2a9cf-1734">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1734">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1735">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1735">Resource</span></span>

* <span data-ttu-id="2a9cf-1736">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1736">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-1737">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1737">Role</span></span>

* <span data-ttu-id="2a9cf-1738">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1738">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="2a9cf-1739">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1739">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="2a9cf-1740">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1740">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1741">SQL</span></span>

* <span data-ttu-id="2a9cf-1742">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1742">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="2a9cf-1743">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1743">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1744">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1744">VM</span></span>

* <span data-ttu-id="2a9cf-1745">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1745">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="2a9cf-1746">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1746">November 14, 2017</span></span>

<span data-ttu-id="2a9cf-1747">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1747">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1748">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1748">ACR</span></span>

* <span data-ttu-id="2a9cf-1749">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1749">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="2a9cf-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1750">ACS</span></span>

* <span data-ttu-id="2a9cf-1751">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1751">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="2a9cf-1752">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1752">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="2a9cf-1753">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1753">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="2a9cf-1754">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1754">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="2a9cf-1755">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1755">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1756">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1756">Appservice</span></span>

* <span data-ttu-id="2a9cf-1757">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1757">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="2a9cf-1758">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1758">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="2a9cf-1759">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1759">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="2a9cf-1760">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1760">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="2a9cf-1761">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1761">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="2a9cf-1762">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1762">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-1763">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1763">Batch</span></span>

* <span data-ttu-id="2a9cf-1764">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1764">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="2a9cf-1765">Batchai</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1765">Batchai</span></span>

* <span data-ttu-id="2a9cf-1766">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1766">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="2a9cf-1767">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1767">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="2a9cf-1768">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1768">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="2a9cf-1769">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1769">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="2a9cf-1770">Cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1770">Cloud</span></span>

* <span data-ttu-id="2a9cf-1771">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1771">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-1772">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1772">Container</span></span>

* <span data-ttu-id="2a9cf-1773">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1773">Added support to open multiple ports</span></span>
* <span data-ttu-id="2a9cf-1774">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1774">Added container group restart policy</span></span>
* <span data-ttu-id="2a9cf-1775">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1775">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="2a9cf-1776">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1776">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2a9cf-1777">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1777">Data Lake Analytics</span></span>

* <span data-ttu-id="2a9cf-1778">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1778">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2a9cf-1779">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1779">Data Lake Store</span></span>

* <span data-ttu-id="2a9cf-1780">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1780">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1781">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1781">Extension</span></span>

* <span data-ttu-id="2a9cf-1782">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1782">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="2a9cf-1783">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1783">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-1784">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1784">IoT</span></span>

* <span data-ttu-id="2a9cf-1785">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1785">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1786">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1786">Monitor</span></span>

* <span data-ttu-id="2a9cf-1787">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1787">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1788">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1788">Network</span></span>

* <span data-ttu-id="2a9cf-1789">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1789">Added support for CAA DNS records</span></span>
* <span data-ttu-id="2a9cf-1790">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1790">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="2a9cf-1791">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1791">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="2a9cf-1792">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1792">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="2a9cf-1793">Réservations</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1793">Reservations</span></span>

* <span data-ttu-id="2a9cf-1794">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1794">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1795">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1795">Resource</span></span>

* <span data-ttu-id="2a9cf-1796">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1796">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1797">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1797">SQL</span></span>

* <span data-ttu-id="2a9cf-1798">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1798">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1799">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1799">Storage</span></span>

* <span data-ttu-id="2a9cf-1800">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1800">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="2a9cf-1801">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1801">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="2a9cf-1802">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1802">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="2a9cf-1803">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1803">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="2a9cf-1804">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1804">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="2a9cf-1805">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1805">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="2a9cf-1806">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1806">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1807">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1807">VM</span></span>

* <span data-ttu-id="2a9cf-1808">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1808">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="2a9cf-1809">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1809">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="2a9cf-1810">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1810">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="2a9cf-1811">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1811">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="2a9cf-1812">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1812">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="2a9cf-1813">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1813">October 24, 2017</span></span>

<span data-ttu-id="2a9cf-1814">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1814">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1815">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1815">Core</span></span>

* <span data-ttu-id="2a9cf-1816">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1816">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-1817">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1817">ACR</span></span>

* <span data-ttu-id="2a9cf-1818">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1818">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="2a9cf-1819">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1819">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="2a9cf-1820">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1820">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1821">ACS</span></span>

* <span data-ttu-id="2a9cf-1822">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1822">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="2a9cf-1823">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1823">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1824">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1824">Appservice</span></span>

* <span data-ttu-id="2a9cf-1825">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1825">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="2a9cf-1826">Composant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1826">Component</span></span>

* <span data-ttu-id="2a9cf-1827">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1827">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-1828">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1828">Monitor</span></span>

* <span data-ttu-id="2a9cf-1829">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1829">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1830">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1830">Resource</span></span>

* <span data-ttu-id="2a9cf-1831">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1831">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="2a9cf-1832">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1832">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1833">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1833">VM</span></span>

* <span data-ttu-id="2a9cf-1834">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1834">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="2a9cf-1835">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1835">October 9, 2017</span></span>

<span data-ttu-id="2a9cf-1836">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1836">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1837">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1837">Core</span></span>

* <span data-ttu-id="2a9cf-1838">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1838">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1839">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1839">Appservice</span></span>

* <span data-ttu-id="2a9cf-1840">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1840">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-1841">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1841">Batch</span></span>

* <span data-ttu-id="2a9cf-1842">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1842">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="2a9cf-1843">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1843">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="2a9cf-1844">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1844">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="2a9cf-1845">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1845">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="2a9cf-1846">Batchai</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1846">Batchai</span></span>

* <span data-ttu-id="2a9cf-1847">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1847">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-1848">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1848">Keyvault</span></span>

* <span data-ttu-id="2a9cf-1849">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1849">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="2a9cf-1850">(#4448)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1850">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="2a9cf-1851">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1851">Network</span></span>

* <span data-ttu-id="2a9cf-1852">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1852">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="2a9cf-1853">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1853">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1854">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1854">Resource</span></span>

* <span data-ttu-id="2a9cf-1855">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1855">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="2a9cf-1856">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1856">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="2a9cf-1857">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1857">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="2a9cf-1858">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1858">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1859">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1859">Sql</span></span>

* <span data-ttu-id="2a9cf-1860">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1860">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="2a9cf-1861">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1861">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="2a9cf-1862">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1862">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1863">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1863">Storage</span></span>

* <span data-ttu-id="2a9cf-1864">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1864">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1865">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1865">Vm</span></span>

* <span data-ttu-id="2a9cf-1866">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1866">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="2a9cf-1867">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1867">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="2a9cf-1868">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1868">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="2a9cf-1869">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1869">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="2a9cf-1870">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1870">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="2a9cf-1871">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1871">September 22, 2017</span></span>

<span data-ttu-id="2a9cf-1872">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1872">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1873">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1873">Resource</span></span>

* <span data-ttu-id="2a9cf-1874">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1874">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="2a9cf-1875">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1875">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="2a9cf-1876">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1876">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="2a9cf-1877">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1877">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1878">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1878">Network</span></span>

* <span data-ttu-id="2a9cf-1879">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1879">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="2a9cf-1880">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1880">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="2a9cf-1881">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1881">Added `asg` application security group commands</span></span>
* <span data-ttu-id="2a9cf-1882">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1882">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="2a9cf-1883">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1883">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1884">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1884">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1885">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1885">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1886">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1886">Storage</span></span>

* <span data-ttu-id="2a9cf-1887">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1887">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2a9cf-1888">Événement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1888">Eventgrid</span></span>

* <span data-ttu-id="2a9cf-1889">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1889">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1890">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1890">SQL</span></span>

* <span data-ttu-id="2a9cf-1891">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1891">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="2a9cf-1892">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1892">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="2a9cf-1893">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1893">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-1894">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1894">Keyvault</span></span>

* <span data-ttu-id="2a9cf-1895">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1895">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1896">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1896">VM</span></span>

* <span data-ttu-id="2a9cf-1897">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1897">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="2a9cf-1898">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1898">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="2a9cf-1899">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1899">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="2a9cf-1900">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1900">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="2a9cf-1901">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1901">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="2a9cf-1902">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1902">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1903">ACS</span></span>

* <span data-ttu-id="2a9cf-1904">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1904">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1905">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1905">Appservice</span></span>

* <span data-ttu-id="2a9cf-1906">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1906">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="2a9cf-1907">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1907">Backup</span></span>

* <span data-ttu-id="2a9cf-1908">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1908">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="2a9cf-1909">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1909">September 11, 2017</span></span>

<span data-ttu-id="2a9cf-1910">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1910">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="2a9cf-1911">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1911">Core</span></span>

* <span data-ttu-id="2a9cf-1912">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1912">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="2a9cf-1913">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1913">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1914">Acs</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1914">Acs</span></span>

* <span data-ttu-id="2a9cf-1915">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1915">Added `acs list-locations` command</span></span>
* <span data-ttu-id="2a9cf-1916">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1916">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1917">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1917">Appservice</span></span>

* <span data-ttu-id="2a9cf-1918">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1918">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-1919">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1919">CDN</span></span>

* <span data-ttu-id="2a9cf-1920">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1920">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="2a9cf-1921">Extension</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1921">Extension</span></span>

* <span data-ttu-id="2a9cf-1922">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1922">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-1923">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1923">Keyvault</span></span>

* <span data-ttu-id="2a9cf-1924">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1924">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1925">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1925">Network</span></span>

* <span data-ttu-id="2a9cf-1926">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1926">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="2a9cf-1927">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1927">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="2a9cf-1928">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1928">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="2a9cf-1929">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1929">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="2a9cf-1930">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1930">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-1931">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1931">Resource</span></span>

* <span data-ttu-id="2a9cf-1932">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1932">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="2a9cf-1933">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1933">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="2a9cf-1934">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1934">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="2a9cf-1935">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1935">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-1936">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1936">SQL</span></span>

* <span data-ttu-id="2a9cf-1937">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1937">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1938">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1938">VM</span></span>

* <span data-ttu-id="2a9cf-1939">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1939">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="2a9cf-1940">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1940">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="2a9cf-1941">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1941">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="2a9cf-1942">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1942">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="2a9cf-1943">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1943">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="2a9cf-1944">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1944">August 31, 2017</span></span>

<span data-ttu-id="2a9cf-1945">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1945">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-1946">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1946">Keyvault</span></span>

* <span data-ttu-id="2a9cf-1947">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1947">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="2a9cf-1948">Sf</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1948">Sf</span></span>

* <span data-ttu-id="2a9cf-1949">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1949">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1950">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1950">Storage</span></span>

* <span data-ttu-id="2a9cf-1951">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1951">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="2a9cf-1952">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1952">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="2a9cf-1953">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1953">August 28, 2017</span></span>

<span data-ttu-id="2a9cf-1954">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1954">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="2a9cf-1955">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1955">CLI</span></span>

* <span data-ttu-id="2a9cf-1956">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1956">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1957">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1957">ACS</span></span>

* <span data-ttu-id="2a9cf-1958">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1958">Corrected preview regions</span></span>
* <span data-ttu-id="2a9cf-1959">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1959">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="2a9cf-1960">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1960">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-1961">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1961">Appservice</span></span>

* <span data-ttu-id="2a9cf-1962">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1962">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="2a9cf-1963">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1963">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="2a9cf-1964">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1964">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="2a9cf-1965">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1965">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="2a9cf-1966">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1966">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-1967">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1967">IoT</span></span>

* <span data-ttu-id="2a9cf-1968">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1968">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-1969">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1969">Network</span></span>

* <span data-ttu-id="2a9cf-1970">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1970">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="2a9cf-1971">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1971">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1972">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1972">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="2a9cf-1973">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1973">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="2a9cf-1974">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1974">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-1975">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1975">Profile</span></span>

* <span data-ttu-id="2a9cf-1976">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1976">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2a9cf-1977">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1977">Service Fabric</span></span>

* <span data-ttu-id="2a9cf-1978">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1978">Preview release</span></span>
* <span data-ttu-id="2a9cf-1979">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1979">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="2a9cf-1980">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1980">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="2a9cf-1981">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1981">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-1982">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1982">Storage</span></span>

* <span data-ttu-id="2a9cf-1983">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1983">Enabled setting blob tier</span></span>
* <span data-ttu-id="2a9cf-1984">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1984">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="2a9cf-1985">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1985">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="2a9cf-1986">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1986">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="2a9cf-1987">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1987">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="2a9cf-1988">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1988">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-1989">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1989">VM</span></span>

* <span data-ttu-id="2a9cf-1990">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1990">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="2a9cf-1991">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1991">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="2a9cf-1992">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1992">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="2a9cf-1993">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1993">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="2a9cf-1994">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1994">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="2a9cf-1995">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1995">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="2a9cf-1996">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1996">August 15, 2017</span></span>

<span data-ttu-id="2a9cf-1997">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1997">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-1998">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1998">ACS</span></span>

* <span data-ttu-id="2a9cf-1999">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-1999">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2000">Appservice</span></span>

* <span data-ttu-id="2a9cf-2001">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2001">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="2a9cf-2002">Event Grid</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2002">Event Grid</span></span>

* <span data-ttu-id="2a9cf-2003">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2003">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="2a9cf-2004">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2004">August 11, 2017</span></span>

<span data-ttu-id="2a9cf-2005">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2005">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-2006">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2006">ACS</span></span>

* <span data-ttu-id="2a9cf-2007">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2007">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-2008">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2008">Batch</span></span>

* <span data-ttu-id="2a9cf-2009">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2009">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="2a9cf-2010">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2010">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="2a9cf-2011">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2011">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="2a9cf-2012">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2012">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="2a9cf-2013">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2013">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="2a9cf-2014">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2014">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="2a9cf-2015">Composant</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2015">Component</span></span>

* <span data-ttu-id="2a9cf-2016">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2016">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="2a9cf-2017">Conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2017">Container</span></span>

* <span data-ttu-id="2a9cf-2018">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2018">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="2a9cf-2019">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2019">Data Lake Store</span></span>

* <span data-ttu-id="2a9cf-2020">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2020">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="2a9cf-2021">Event Grid</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2021">Event Grid</span></span>

* <span data-ttu-id="2a9cf-2022">Version initiale</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2022">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-2023">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2023">Network</span></span>

* <span data-ttu-id="2a9cf-2024">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2024">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="2a9cf-2025">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2025">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="2a9cf-2026">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2026">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="2a9cf-2027">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2027">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-2028">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2028">Profile</span></span>

* <span data-ttu-id="2a9cf-2029">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2029">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-2030">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2030">Storage</span></span>

* <span data-ttu-id="2a9cf-2031">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2031">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-2032">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2032">VM</span></span>

* <span data-ttu-id="2a9cf-2033">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2033">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="2a9cf-2034">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2034">Exposed `list-skus` command</span></span>
* <span data-ttu-id="2a9cf-2035">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2035">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="2a9cf-2036">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2036">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="2a9cf-2037">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2037">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="2a9cf-2038">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2038">July 28, 2017</span></span>

<span data-ttu-id="2a9cf-2039">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2039">Version 2.0.12</span></span>

* <span data-ttu-id="2a9cf-2040">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2040">Added container commands</span></span>
* <span data-ttu-id="2a9cf-2041">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2041">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="2a9cf-2042">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2042">Core</span></span>

* <span data-ttu-id="2a9cf-2043">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2043">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="2a9cf-2044">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2044">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="2a9cf-2045">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2045">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="2a9cf-2046">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2046">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="2a9cf-2047">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2047">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="2a9cf-2048">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2048">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="2a9cf-2049">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2049">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="2a9cf-2050">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2050">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="2a9cf-2051">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2051">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="2a9cf-2052">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2052">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="2a9cf-2053">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2053">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="2a9cf-2054">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2054">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="2a9cf-2055">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2055">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="2a9cf-2056">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2056">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="2a9cf-2057">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2057">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="2a9cf-2058">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2058">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="2a9cf-2059">ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2059">ACR</span></span>

* <span data-ttu-id="2a9cf-2060">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2060">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="2a9cf-2061">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2061">Support SKU update for managed registries</span></span>
* <span data-ttu-id="2a9cf-2062">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2062">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="2a9cf-2063">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2063">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="2a9cf-2064">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2064">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="2a9cf-2065">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2065">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-2066">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2066">ACS</span></span>

* <span data-ttu-id="2a9cf-2067">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2067">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-2068">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2068">Appservice</span></span>

* <span data-ttu-id="2a9cf-2069">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2069">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="2a9cf-2070">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2070">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="2a9cf-2071">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2071">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="2a9cf-2072">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2072">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="2a9cf-2073">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2073">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="2a9cf-2074">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2074">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="2a9cf-2075">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2075">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="2a9cf-2076">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2076">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="2a9cf-2077">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2077">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="2a9cf-2078">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2078">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="2a9cf-2079">Batch</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2079">Batch</span></span>

* <span data-ttu-id="2a9cf-2080">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2080">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="2a9cf-2081">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2081">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="2a9cf-2082">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2082">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="2a9cf-2083">CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2083">CDN</span></span>

* <span data-ttu-id="2a9cf-2084">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2084">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="2a9cf-2085">Cloud</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2085">Cloud</span></span>

* <span data-ttu-id="2a9cf-2086">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2086">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="2a9cf-2087">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2087">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="2a9cf-2088">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2088">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="2a9cf-2089">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2089">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="2a9cf-2090">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2090">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-2091">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2091">CosmosDB</span></span>

* <span data-ttu-id="2a9cf-2092">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2092">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="2a9cf-2093">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2093">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2a9cf-2094">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2094">Data Lake Analytics</span></span>

* <span data-ttu-id="2a9cf-2095">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2095">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="2a9cf-2096">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2096">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="2a9cf-2097">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2097">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2a9cf-2098">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2098">Data Lake Store</span></span>

* <span data-ttu-id="2a9cf-2099">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2099">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="2a9cf-2100">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2100">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="2a9cf-2101">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2101">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="2a9cf-2102">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2102">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="2a9cf-2103">Interactive</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2103">Interactive</span></span>

* <span data-ttu-id="2a9cf-2104">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2104">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="2a9cf-2105">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2105">Increased test coverage</span></span>
* <span data-ttu-id="2a9cf-2106">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2106">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="2a9cf-2107">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2107">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="2a9cf-2108">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2108">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="2a9cf-2109">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2109">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="2a9cf-2110">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2110">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="2a9cf-2111">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2111">Added `--progress` flag</span></span>
* <span data-ttu-id="2a9cf-2112">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2112">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="2a9cf-2113">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2113">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="2a9cf-2114">IoT</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2114">IoT</span></span>

* <span data-ttu-id="2a9cf-2115">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2115">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="2a9cf-2116">(#3934)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2116">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="2a9cf-2117">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2117">Key vault</span></span>

* <span data-ttu-id="2a9cf-2118">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2118">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="2a9cf-2119">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2119">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="2a9cf-2120">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2120">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="2a9cf-2121">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2121">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="2a9cf-2122">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2122">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="2a9cf-2123">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2123">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="2a9cf-2124">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2124">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="2a9cf-2125">(#3307)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2125">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="2a9cf-2126">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2126">Lab</span></span>

* <span data-ttu-id="2a9cf-2127">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2127">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="2a9cf-2128">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2128">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-2129">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2129">Monitor</span></span>

* <span data-ttu-id="2a9cf-2130">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2130">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="2a9cf-2131">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2131">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="2a9cf-2132">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2132">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="2a9cf-2133">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2133">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="2a9cf-2134">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2134">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="2a9cf-2135">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2135">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="2a9cf-2136">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2136">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="2a9cf-2137">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2137">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="2a9cf-2138">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2138">`location` no longer required</span></span>
  * <span data-ttu-id="2a9cf-2139">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2139">Add name and ID support for target</span></span>
  * <span data-ttu-id="2a9cf-2140">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2140">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="2a9cf-2141">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2141">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="2a9cf-2142">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2142">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="2a9cf-2143">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2143">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="2a9cf-2144">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2144">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="2a9cf-2145">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2145">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-2146">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2146">Network</span></span>

* <span data-ttu-id="2a9cf-2147">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2147">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="2a9cf-2148">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2148">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="2a9cf-2149">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2149">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="2a9cf-2150">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2150">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="2a9cf-2151">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2151">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="2a9cf-2152">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2152">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="2a9cf-2153">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2153">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="2a9cf-2154">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2154">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="2a9cf-2155">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2155">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="2a9cf-2156">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2156">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="2a9cf-2157">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2157">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="2a9cf-2158">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2158">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="2a9cf-2159">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2159">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="2a9cf-2160">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2160">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="2a9cf-2161">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2161">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="2a9cf-2162">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2162">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="2a9cf-2163">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2163">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="2a9cf-2164">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2164">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="2a9cf-2165">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2165">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="2a9cf-2166">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2166">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="2a9cf-2167">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2167">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="2a9cf-2168">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2168">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="2a9cf-2169">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2169">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="2a9cf-2170">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2170">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="2a9cf-2171">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2171">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="2a9cf-2172">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2172">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="2a9cf-2173">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2173">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-2174">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2174">Profile</span></span>

* <span data-ttu-id="2a9cf-2175">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2175">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="2a9cf-2176">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2176">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="2a9cf-2177">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2177">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="2a9cf-2178">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2178">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="2a9cf-2179">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2179">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="2a9cf-2180">SGBDR</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2180">RDBMS</span></span>

* <span data-ttu-id="2a9cf-2181">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2181">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="2a9cf-2182">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2182">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="2a9cf-2183">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2183">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="2a9cf-2184">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2184">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-2185">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2185">Resource</span></span>

* <span data-ttu-id="2a9cf-2186">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2186">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="2a9cf-2187">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2187">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="2a9cf-2188">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2188">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="2a9cf-2189">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2189">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="2a9cf-2190">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2190">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="2a9cf-2191">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2191">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="2a9cf-2192">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2192">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="2a9cf-2193">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2193">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-2194">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2194">Role</span></span>

* <span data-ttu-id="2a9cf-2195">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2195">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="2a9cf-2196">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2196">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="2a9cf-2197">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2197">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="2a9cf-2198">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2198">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="2a9cf-2199">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2199">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2a9cf-2200">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2200">Service Fabric</span></span>
* <span data-ttu-id="2a9cf-2201">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2201">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="2a9cf-2202">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2202">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="2a9cf-2203">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2203">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-2204">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2204">SQL</span></span>

* <span data-ttu-id="2a9cf-2205">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2205">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="2a9cf-2206">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2206">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="2a9cf-2207">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2207">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-2208">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2208">Storage</span></span>

* <span data-ttu-id="2a9cf-2209">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2209">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="2a9cf-2210">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2210">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="2a9cf-2211">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2211">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="2a9cf-2212">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2212">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="2a9cf-2213">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2213">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="2a9cf-2214">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2214">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-2215">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2215">VM</span></span>

* <span data-ttu-id="2a9cf-2216">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2216">Support configuring nsg</span></span>
* <span data-ttu-id="2a9cf-2217">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2217">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="2a9cf-2218">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2218">Support managed service identities</span></span>
* <span data-ttu-id="2a9cf-2219">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2219">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="2a9cf-2220">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2220">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="2a9cf-2221">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2221">May 10, 2017</span></span>

<span data-ttu-id="2a9cf-2222">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2222">Version 2.0.6</span></span>

* <span data-ttu-id="2a9cf-2223">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2223">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="2a9cf-2224">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2224">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="2a9cf-2225">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2225">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="2a9cf-2226">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2226">Include Cognitive Services module</span></span>
* <span data-ttu-id="2a9cf-2227">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2227">Include Service Fabric module</span></span>
* <span data-ttu-id="2a9cf-2228">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2228">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="2a9cf-2229">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2229">Add support for CDN commands</span></span>
* <span data-ttu-id="2a9cf-2230">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2230">Remove Container module</span></span>
* <span data-ttu-id="2a9cf-2231">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2231">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="2a9cf-2232">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2232">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="2a9cf-2233">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2233">Core</span></span>

* <span data-ttu-id="2a9cf-2234">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2234">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="2a9cf-2235">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2235">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="2a9cf-2236">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2236">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="2a9cf-2237">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2237">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="2a9cf-2238">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2238">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="2a9cf-2239">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2239">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="2a9cf-2240">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2240">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="2a9cf-2241">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2241">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="2a9cf-2242">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2242">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="2a9cf-2243">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2243">core: Improved performance</span></span>
* <span data-ttu-id="2a9cf-2244">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2244">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="2a9cf-2245">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2245">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2246">ACS</span></span>

* <span data-ttu-id="2a9cf-2247">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2247">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="2a9cf-2248">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2248">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="2a9cf-2249">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2249">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="2a9cf-2250">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2250">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-2251">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2251">AppService</span></span>

* <span data-ttu-id="2a9cf-2252">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2252">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="2a9cf-2253">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2253">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="2a9cf-2254">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2254">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="2a9cf-2255">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2255">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="2a9cf-2256">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2256">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="2a9cf-2257">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2257">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="2a9cf-2258">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2258">support slot swap with preview</span></span>
* <span data-ttu-id="2a9cf-2259">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2259">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="2a9cf-2260">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2260">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2a9cf-2261">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2261">CosmosDB</span></span>

* <span data-ttu-id="2a9cf-2262">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2262">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="2a9cf-2263">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2263">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="2a9cf-2264">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2264">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="2a9cf-2265">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2265">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2a9cf-2266">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2266">Data Lake Analytics</span></span>

* <span data-ttu-id="2a9cf-2267">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2267">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="2a9cf-2268">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2268">Add support for new catalog item type: package.</span></span> <span data-ttu-id="2a9cf-2269">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2269">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="2a9cf-2270">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2270">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="2a9cf-2271">Table</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2271">Table</span></span>
  * <span data-ttu-id="2a9cf-2272">Fonction table</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2272">Table valued function</span></span>
  * <span data-ttu-id="2a9cf-2273">Affichage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2273">View</span></span>
  * <span data-ttu-id="2a9cf-2274">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2274">Table Statistics.</span></span> <span data-ttu-id="2a9cf-2275">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2275">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2a9cf-2276">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2276">Data Lake Store</span></span>

* <span data-ttu-id="2a9cf-2277">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2277">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="2a9cf-2278">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2278">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="2a9cf-2279">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2279">missed help for access show.</span></span> <span data-ttu-id="2a9cf-2280">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2280">adding it.</span></span> <span data-ttu-id="2a9cf-2281">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2281">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="2a9cf-2282">Rechercher</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2282">Find</span></span>

* <span data-ttu-id="2a9cf-2283">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2283">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="2a9cf-2284">KeyVault</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2284">KeyVault</span></span>

* <span data-ttu-id="2a9cf-2285">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2285">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="2a9cf-2286">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2286">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="2a9cf-2287">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2287">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="2a9cf-2288">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2288">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="2a9cf-2289">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2289">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="2a9cf-2290">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2290">Lab</span></span>

* <span data-ttu-id="2a9cf-2291">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2291">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="2a9cf-2292">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2292">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="2a9cf-2293">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2293">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="2a9cf-2294">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2294">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="2a9cf-2295">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2295">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="2a9cf-2296">Surveiller</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2296">Monitor</span></span>

* <span data-ttu-id="2a9cf-2297">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2297">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="2a9cf-2298">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2298">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="2a9cf-2299">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2299">Network</span></span>

* <span data-ttu-id="2a9cf-2300">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2300">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="2a9cf-2301">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2301">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="2a9cf-2302">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2302">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="2a9cf-2303">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2303">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="2a9cf-2304">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2304">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="2a9cf-2305">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2305">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="2a9cf-2306">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2306">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="2a9cf-2307">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2307">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="2a9cf-2308">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2308">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="2a9cf-2309">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2309">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="2a9cf-2310">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2310">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="2a9cf-2311">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2311">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="2a9cf-2312">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2312">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="2a9cf-2313">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2313">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="2a9cf-2314">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2314">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="2a9cf-2315">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2315">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="2a9cf-2316">Profil</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2316">Profile</span></span>

* <span data-ttu-id="2a9cf-2317">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2317">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="2a9cf-2318">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2318">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="2a9cf-2319">Redis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2319">Redis</span></span>

* <span data-ttu-id="2a9cf-2320">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2320">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="2a9cf-2321">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2321">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="2a9cf-2322">Ressource</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2322">Resource</span></span>

* <span data-ttu-id="2a9cf-2323">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2323">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="2a9cf-2324">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2324">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="2a9cf-2325">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2325">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="2a9cf-2326">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2326">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="2a9cf-2327">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2327">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="2a9cf-2328">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2328">Add docs for az lock update.</span></span> <span data-ttu-id="2a9cf-2329">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2329">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="2a9cf-2330">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2330">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="2a9cf-2331">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2331">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="2a9cf-2332">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2332">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="2a9cf-2333">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2333">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="2a9cf-2334">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2334">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="2a9cf-2335">Rôle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2335">Role</span></span>

* <span data-ttu-id="2a9cf-2336">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2336">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="2a9cf-2337">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2337">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="2a9cf-2338">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2338">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="2a9cf-2339">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2339">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="2a9cf-2340">SQL</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2340">SQL</span></span>

* <span data-ttu-id="2a9cf-2341">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2341">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="2a9cf-2342">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2342">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="2a9cf-2343">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2343">Storage</span></span>

* <span data-ttu-id="2a9cf-2344">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2344">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="2a9cf-2345">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2345">Add support for incremental blob copy</span></span>
* <span data-ttu-id="2a9cf-2346">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2346">Add support for large block blob upload</span></span>
* <span data-ttu-id="2a9cf-2347">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2347">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-2348">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2348">VM</span></span>

* <span data-ttu-id="2a9cf-2349">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2349">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="2a9cf-2350">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2350">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="2a9cf-2351">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2351">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="2a9cf-2352">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2352">az vm/vmss disk</span></span>
  3. <span data-ttu-id="2a9cf-2353">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2353">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="2a9cf-2354">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2354">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="2a9cf-2355">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2355">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="2a9cf-2356">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2356">April 3, 2017</span></span>

<span data-ttu-id="2a9cf-2357">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2357">Version 2.0.2</span></span>

<span data-ttu-id="2a9cf-2358">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2358">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="2a9cf-2359">Principal</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2359">Core</span></span>

* <span data-ttu-id="2a9cf-2360">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2360">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="2a9cf-2361">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2361">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="2a9cf-2362">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2362">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="2a9cf-2363">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2363">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="2a9cf-2364">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2364">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="2a9cf-2365">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2365">Add prompting for missing template parameters.</span></span> <span data-ttu-id="2a9cf-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="2a9cf-2367">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2367">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="2a9cf-2368">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2368">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="2a9cf-2369">ACS</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2369">ACS</span></span>

* <span data-ttu-id="2a9cf-2370">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2370">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="2a9cf-2371">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2371">Add support for ssh key password prompting.</span></span> <span data-ttu-id="2a9cf-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="2a9cf-2373">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2373">Add support for windows clusters.</span></span> <span data-ttu-id="2a9cf-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="2a9cf-2375">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2375">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="2a9cf-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="2a9cf-2377">AppService</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2377">AppService</span></span>

* <span data-ttu-id="2a9cf-2378">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2378">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="2a9cf-2379">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2379">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="2a9cf-2380">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2380">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="2a9cf-2381">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2381">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="2a9cf-2382">DataLake</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2382">DataLake</span></span>

* <span data-ttu-id="2a9cf-2383">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2383">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="2a9cf-2384">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2384">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="2a9cf-2385">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2385">DocuemntDB</span></span>

* <span data-ttu-id="2a9cf-2386">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2386">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="2a9cf-2387">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2387">VM</span></span>

* <span data-ttu-id="2a9cf-2388">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2388">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="2a9cf-2389">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2389">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="2a9cf-2390">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2390">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="2a9cf-2391">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2391">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="2a9cf-2392">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2392">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="2a9cf-2393">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2393">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="2a9cf-2394">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2394">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="2a9cf-2395">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2395">February 27, 2017</span></span>

<span data-ttu-id="2a9cf-2396">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2396">Version 2.0.0</span></span>

<span data-ttu-id="2a9cf-2397">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2397">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="2a9cf-2398">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2398">Container Service (acs)</span></span>
- <span data-ttu-id="2a9cf-2399">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2399">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="2a9cf-2400">Réseau</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2400">Networking</span></span>
- <span data-ttu-id="2a9cf-2401">Stockage</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2401">Storage</span></span>

<span data-ttu-id="2a9cf-2402">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2402">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="2a9cf-2403">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2403">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="2a9cf-2404">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2404">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="2a9cf-2405">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2405">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="2a9cf-2406">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2406">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="2a9cf-2407">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2407">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="2a9cf-2408">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2408">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="2a9cf-2409">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2409">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="2a9cf-2410">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="2a9cf-2410">Provide feedback from the command line with the `az feedback` command</span></span>

