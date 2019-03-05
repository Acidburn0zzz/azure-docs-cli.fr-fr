---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9f35084eeecab491e5be63eb856b0bb64a6157d0
ms.sourcegitcommit: 9fb008f2802ca6a58f33e01263bf55a80d01f031
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/27/2019
ms.locfileid: "56891209"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="00039-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="00039-103">Azure CLI release notes</span></span>
## <a name="february-26-2019"></a><span data-ttu-id="00039-104">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="00039-104">February 26, 2019</span></span>

<span data-ttu-id="00039-105">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="00039-105">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="00039-106">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-106">Core</span></span>

* <span data-ttu-id="00039-107">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="00039-107">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="00039-108">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-108">ACR</span></span>

* <span data-ttu-id="00039-109">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="00039-109">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="00039-110">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="00039-110">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="00039-111">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-111">ACS</span></span>

* <span data-ttu-id="00039-112">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="00039-112">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-113">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-113">AppService</span></span>

* <span data-ttu-id="00039-114">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="00039-114">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="00039-115">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-115">Batch</span></span>
* <span data-ttu-id="00039-116">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="00039-116">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="00039-117">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="00039-117">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="00039-118">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="00039-118">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="00039-119">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="00039-119">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="00039-120">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="00039-120">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="00039-121">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="00039-121">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-122">CosmosDB</span></span>

* <span data-ttu-id="00039-123">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="00039-123">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="00039-124">Kusto</span><span class="sxs-lookup"><span data-stu-id="00039-124">Kusto</span></span>

* <span data-ttu-id="00039-125">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="00039-125">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="00039-126">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-126">Network</span></span>

* <span data-ttu-id="00039-127">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-127">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="00039-128">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="00039-128">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="00039-129">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="00039-129">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="00039-130">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-130">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="00039-131">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-131">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="00039-132">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-132">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="00039-133">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="00039-133">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="00039-134">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-134">Resource</span></span>

* <span data-ttu-id="00039-135">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="00039-135">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="00039-136">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="00039-136">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="00039-137">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="00039-137">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="00039-138">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="00039-138">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="00039-139">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-139">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="00039-140">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-140">Role</span></span>

* <span data-ttu-id="00039-141">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-141">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-142">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-142">VM</span></span>

* <span data-ttu-id="00039-143">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="00039-143">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="00039-144">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="00039-144">February 12, 2019</span></span>

<span data-ttu-id="00039-145">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="00039-145">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="00039-146">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-146">Core</span></span>

* <span data-ttu-id="00039-147">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="00039-147">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="00039-148">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="00039-148">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="00039-149">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-149">ACR</span></span>
* <span data-ttu-id="00039-150">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="00039-150">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="00039-151">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="00039-151">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="00039-152">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-152">ACS</span></span>
* <span data-ttu-id="00039-153">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="00039-153">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="00039-154">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="00039-154">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="00039-155">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="00039-155">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="00039-156">AMS</span><span class="sxs-lookup"><span data-stu-id="00039-156">AMS</span></span>
* <span data-ttu-id="00039-157">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="00039-157">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="00039-158">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="00039-158">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-159">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-159">Appservice</span></span>
* <span data-ttu-id="00039-160">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="00039-160">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="00039-161">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="00039-161">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="00039-162">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="00039-162">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="00039-163">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="00039-163">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="00039-164">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="00039-164">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="00039-165">Botservice</span><span class="sxs-lookup"><span data-stu-id="00039-165">Botservice</span></span>
* <span data-ttu-id="00039-166">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="00039-166">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="00039-167">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="00039-167">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="00039-168">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="00039-168">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="00039-169">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="00039-169">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="00039-170">[DÉPRÉCIÉ] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="00039-170">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="00039-171">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="00039-171">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="00039-172">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="00039-172">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="00039-173">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="00039-173">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="00039-174">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="00039-174">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="00039-175">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="00039-175">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="00039-176">Key Vault</span><span class="sxs-lookup"><span data-stu-id="00039-176">Key Vault</span></span>
* <span data-ttu-id="00039-177">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="00039-177">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-178">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-178">Monitor</span></span>
* <span data-ttu-id="00039-179">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="00039-179">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="00039-180">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-180">Network</span></span>
* <span data-ttu-id="00039-181">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="00039-181">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="00039-182">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="00039-182">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="00039-183">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="00039-183">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="00039-184">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-184">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="00039-185">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="00039-185">Policy Insights</span></span>
* <span data-ttu-id="00039-186">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="00039-186">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-187">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-187">RDBMS</span></span>
* <span data-ttu-id="00039-188">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="00039-188">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="00039-189">Redis</span><span class="sxs-lookup"><span data-stu-id="00039-189">Redis</span></span>
* <span data-ttu-id="00039-190">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="00039-190">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="00039-191">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="00039-191">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="00039-192">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="00039-192">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="00039-193">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="00039-193">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="00039-194">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="00039-194">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="00039-195">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="00039-195">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="00039-196">[DÉPRÉCIÉ] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="00039-196">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="00039-197">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-197">Role</span></span>
* <span data-ttu-id="00039-198">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="00039-198">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="00039-199">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="00039-199">SQL VM</span></span>
* <span data-ttu-id="00039-200">[DÉPRÉCIÉ] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="00039-200">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="00039-201">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-201">VM</span></span>
* <span data-ttu-id="00039-202">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="00039-202">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="00039-203">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="00039-203">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="00039-204">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="00039-204">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="00039-205">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="00039-205">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="00039-206">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="00039-206">January 31, 2019</span></span>

<span data-ttu-id="00039-207">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="00039-207">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="00039-208">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-208">Core</span></span>

* <span data-ttu-id="00039-209">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="00039-209">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="00039-210">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="00039-210">January 28, 2019</span></span>

<span data-ttu-id="00039-211">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="00039-211">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="00039-212">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-212">ACR</span></span>
* <span data-ttu-id="00039-213">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="00039-213">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="00039-214">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-214">ACS</span></span>
* <span data-ttu-id="00039-215">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="00039-215">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="00039-216">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="00039-216">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="00039-217">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="00039-217">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="00039-218">AMS</span><span class="sxs-lookup"><span data-stu-id="00039-218">AMS</span></span>
* <span data-ttu-id="00039-219">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="00039-219">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="00039-220">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="00039-220">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-221">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-221">Appservice</span></span>
* <span data-ttu-id="00039-222">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="00039-222">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="00039-223">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="00039-223">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="00039-224">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="00039-224">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="00039-225">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-225">Container</span></span>
* <span data-ttu-id="00039-226">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="00039-226">Added `container start` command</span></span>
* <span data-ttu-id="00039-227">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-227">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="00039-228">EventGrid</span><span class="sxs-lookup"><span data-stu-id="00039-228">EventGrid</span></span>
* <span data-ttu-id="00039-229">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-229">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="00039-230">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="00039-230">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="00039-231">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="00039-231">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="00039-232">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="00039-232">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="00039-233">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="00039-233">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="00039-234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="00039-234">HDInsight</span></span>
* <span data-ttu-id="00039-235">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="00039-235">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="00039-236">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="00039-236">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="00039-237">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="00039-237">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="00039-238">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="00039-238">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="00039-239">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="00039-239">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="00039-240">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="00039-240">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="00039-241">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-241">IoT</span></span>
* <span data-ttu-id="00039-242">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="00039-242">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="00039-243">Kusto</span><span class="sxs-lookup"><span data-stu-id="00039-243">Kusto</span></span>
* <span data-ttu-id="00039-244">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="00039-244">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-245">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-245">Monitor</span></span>
* <span data-ttu-id="00039-246">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="00039-246">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="00039-247">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-247">Profile</span></span>
* <span data-ttu-id="00039-248">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="00039-248">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="00039-249">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-249">Network</span></span>
* <span data-ttu-id="00039-250">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="00039-250">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="00039-251">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="00039-251">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="00039-252">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-252">Resource</span></span>
* <span data-ttu-id="00039-253">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="00039-253">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="00039-254">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-254">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="00039-255">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="00039-255">SQL Virtual Machine</span></span>
* <span data-ttu-id="00039-256">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="00039-256">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="00039-257">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-257">Storage</span></span>
* <span data-ttu-id="00039-258">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="00039-258">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="00039-259">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="00039-259">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="00039-260">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-260">VM</span></span>
* <span data-ttu-id="00039-261">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="00039-261">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="00039-262">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="00039-262">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="00039-263">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="00039-263">January 15, 2019</span></span>

<span data-ttu-id="00039-264">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="00039-264">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="00039-265">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-265">ACR</span></span>
* <span data-ttu-id="00039-266">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="00039-266">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="00039-267">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="00039-267">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="00039-268">[DÉPRÉCIÉ] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="00039-268">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="00039-269">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-269">ACS</span></span>
* <span data-ttu-id="00039-270">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="00039-270">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-271">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-271">Appservice</span></span>
* <span data-ttu-id="00039-272">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="00039-272">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="00039-273">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="00039-273">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="00039-274">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="00039-274">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="00039-275">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="00039-275">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="00039-276">Botservice</span><span class="sxs-lookup"><span data-stu-id="00039-276">Botservice</span></span>
* <span data-ttu-id="00039-277">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="00039-277">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="00039-278">Configuration</span><span class="sxs-lookup"><span data-stu-id="00039-278">Configure</span></span>
* <span data-ttu-id="00039-279">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="00039-279">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-280">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-280">CosmosDB</span></span>
* <span data-ttu-id="00039-281">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="00039-281">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="00039-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="00039-282">HDInsight</span></span>
* <span data-ttu-id="00039-283">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="00039-283">Added commands for managing applications</span></span>
* <span data-ttu-id="00039-284">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="00039-284">Added commands for managing script actions</span></span>
* <span data-ttu-id="00039-285">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="00039-285">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="00039-286">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="00039-286">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="00039-287">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="00039-287">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="00039-288">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-288">Network</span></span>
* <span data-ttu-id="00039-289">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-289">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="00039-290">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="00039-290">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="00039-291">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-291">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="00039-292">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="00039-292">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="00039-293">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-293">Role</span></span>
* <span data-ttu-id="00039-294">[DÉPRÉCIÉ] Dépréciation de l’argument `--password` au profit de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="00039-294">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="00039-295">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="00039-295">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="00039-296">Sécurité</span><span class="sxs-lookup"><span data-stu-id="00039-296">Security</span></span>
* <span data-ttu-id="00039-297">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-297">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="00039-298">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-298">Storage</span></span>
* <span data-ttu-id="00039-299">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="00039-299">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="00039-300">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="00039-300">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="00039-301">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="00039-301">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="00039-302">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="00039-302">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="00039-303">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="00039-303">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="00039-304">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-304">VM</span></span>
* <span data-ttu-id="00039-305">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="00039-305">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="00039-306">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-306">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="00039-307">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="00039-307">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="00039-308">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="00039-308">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="00039-309">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-309">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="00039-310">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="00039-310">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="00039-311">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-311">December 20, 2018</span></span>

<span data-ttu-id="00039-312">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="00039-312">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="00039-313">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-313">Appservice</span></span>
* <span data-ttu-id="00039-314">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="00039-314">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="00039-315">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="00039-315">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="00039-316">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="00039-316">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="00039-317">IotCentral</span><span class="sxs-lookup"><span data-stu-id="00039-317">IoTCentral</span></span>
* <span data-ttu-id="00039-318">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="00039-318">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="00039-319">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-319">Role</span></span>
* <span data-ttu-id="00039-320">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="00039-320">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="00039-321">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-321">SQL</span></span>
* <span data-ttu-id="00039-322">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="00039-322">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="00039-323">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-323">VM</span></span>
* <span data-ttu-id="00039-324">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="00039-324">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="00039-325">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-325">December 18, 2018</span></span>

<span data-ttu-id="00039-326">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="00039-326">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="00039-327">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-327">ACR</span></span>
* <span data-ttu-id="00039-328">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="00039-328">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="00039-329">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="00039-329">Condensed the table layout for task list</span></span>
* <span data-ttu-id="00039-330">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="00039-330">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="00039-331">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-331">ACS</span></span>
* <span data-ttu-id="00039-332">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="00039-332">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="00039-333">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-333">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="00039-334">[DÉCONSEILLÉ] Commandes `az acs` déconseillées.</span><span class="sxs-lookup"><span data-stu-id="00039-334">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="00039-335">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="00039-335">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="00039-336">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="00039-336">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="00039-337">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="00039-337">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-338">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-338">Appservice</span></span>
* <span data-ttu-id="00039-339">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="00039-339">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="00039-340">Botservice</span><span class="sxs-lookup"><span data-stu-id="00039-340">Botservice</span></span>
* <span data-ttu-id="00039-341">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="00039-341">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="00039-342">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="00039-342">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="00039-343">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="00039-343">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="00039-344">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="00039-344">Reduced Kudu network calls</span></span>
* <span data-ttu-id="00039-345">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="00039-345">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-346">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-346">Consumption</span></span>
* <span data-ttu-id="00039-347">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="00039-347">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-348">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-348">CosmosDB</span></span>
* <span data-ttu-id="00039-349">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="00039-349">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="00039-350">Cartes</span><span class="sxs-lookup"><span data-stu-id="00039-350">Maps</span></span>
* <span data-ttu-id="00039-351">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-351">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="00039-352">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-352">Network</span></span>
* <span data-ttu-id="00039-353">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="00039-353">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="00039-354">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="00039-354">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="00039-355">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-355">Resource</span></span>
* <span data-ttu-id="00039-356">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-356">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="00039-357">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="00039-357">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-358">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-358">Storage</span></span>
*  <span data-ttu-id="00039-359">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="00039-359">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-360">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-360">VM</span></span>
* <span data-ttu-id="00039-361">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="00039-361">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="00039-362">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-362">December 4, 2018</span></span>

<span data-ttu-id="00039-363">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="00039-363">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="00039-364">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-364">Core</span></span>
* <span data-ttu-id="00039-365">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="00039-365">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="00039-366">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="00039-366">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-367">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-367">Appservice</span></span>
* <span data-ttu-id="00039-368">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="00039-368">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="00039-369">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="00039-369">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="00039-370">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-370">Network</span></span>
* <span data-ttu-id="00039-371">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="00039-371">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="00039-372">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-372">Role</span></span>
* <span data-ttu-id="00039-373">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="00039-373">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="00039-374">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-374">VM</span></span>
* <span data-ttu-id="00039-375">[DÉCONSEILLÉ] Le paramètre `vm extension [show|wait] --expand` est déconseillé</span><span class="sxs-lookup"><span data-stu-id="00039-375">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="00039-376">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="00039-376">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="00039-377">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="00039-377">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="00039-378">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="00039-378">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="00039-379">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-379">November 20, 2018</span></span>

<span data-ttu-id="00039-380">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="00039-380">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="00039-381">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-381">Core</span></span>
* <span data-ttu-id="00039-382">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="00039-382">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="00039-383">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-383">ACR</span></span>
* <span data-ttu-id="00039-384">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="00039-384">Added context token to task step</span></span>
* <span data-ttu-id="00039-385">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="00039-385">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="00039-386">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="00039-386">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-387">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-387">Appservice</span></span>
* <span data-ttu-id="00039-388">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="00039-388">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="00039-389">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="00039-389">Updated the default `node_version`.</span></span> <span data-ttu-id="00039-390">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="00039-390">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="00039-391">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="00039-391">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="00039-392">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="00039-392">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="00039-393">IotCentral</span><span class="sxs-lookup"><span data-stu-id="00039-393">IotCentral</span></span>
* <span data-ttu-id="00039-394">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="00039-394">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-395">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-395">KeyVault</span></span>
* <span data-ttu-id="00039-396">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="00039-396">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="00039-397">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-397">Network</span></span>
* <span data-ttu-id="00039-398">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="00039-398">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="00039-399">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="00039-399">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="00039-400">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="00039-400">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="00039-401">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="00039-401">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-402">Rdbms</span><span class="sxs-lookup"><span data-stu-id="00039-402">Rdbms</span></span>
* <span data-ttu-id="00039-403">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="00039-403">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="00039-404">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="00039-404">Rbac</span></span>
* <span data-ttu-id="00039-405">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="00039-405">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="00039-406">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="00039-406">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="00039-407">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-407">Storage</span></span>
* <span data-ttu-id="00039-408">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="00039-408">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="00039-409">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="00039-409">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="00039-410">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="00039-410">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="00039-411">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="00039-411">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="00039-412">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-412">VM</span></span>
* <span data-ttu-id="00039-413">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="00039-413">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="00039-414">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="00039-414">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="00039-415">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="00039-415">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="00039-416">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="00039-416">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="00039-417">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="00039-417">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="00039-418">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="00039-418">Added `snapshot wait` command</span></span>
* <span data-ttu-id="00039-419">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="00039-419">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="00039-420">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-420">November 6, 2018</span></span>

<span data-ttu-id="00039-421">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="00039-421">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="00039-422">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-422">Core</span></span>
* <span data-ttu-id="00039-423">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="00039-423">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="00039-424">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-424">ACR</span></span>
* <span data-ttu-id="00039-425">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="00039-425">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="00039-426">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="00039-426">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="00039-427">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-427">ACS</span></span>
* <span data-ttu-id="00039-428">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-428">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="00039-429">Advisor</span><span class="sxs-lookup"><span data-stu-id="00039-429">Advisor</span></span>
* <span data-ttu-id="00039-430">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="00039-430">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="00039-431">AMS</span><span class="sxs-lookup"><span data-stu-id="00039-431">AMS</span></span>
* <span data-ttu-id="00039-432">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="00039-432">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="00039-433">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="00039-433">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="00039-434">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="00039-434">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="00039-435">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="00039-435">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="00039-436">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="00039-436">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="00039-437">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="00039-437">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="00039-438">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="00039-438">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="00039-439">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="00039-439">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="00039-440">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="00039-440">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="00039-441">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="00039-441">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="00039-442">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="00039-442">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="00039-443">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="00039-443">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="00039-444">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="00039-444">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="00039-445">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="00039-445">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="00039-446">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="00039-446">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="00039-447">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="00039-447">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="00039-448">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="00039-448">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-449">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-449">AppService</span></span>
* <span data-ttu-id="00039-450">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="00039-450">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="00039-451">Configuration</span><span class="sxs-lookup"><span data-stu-id="00039-451">Configure</span></span>
* <span data-ttu-id="00039-452">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="00039-452">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="00039-453">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-453">Container</span></span>
* <span data-ttu-id="00039-454">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="00039-454">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="00039-455">Event Hub</span><span class="sxs-lookup"><span data-stu-id="00039-455">EventHub</span></span>
* <span data-ttu-id="00039-456">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-456">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-457">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-457">Interactive</span></span>
* <span data-ttu-id="00039-458">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="00039-458">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-459">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-459">Monitor</span></span>
* <span data-ttu-id="00039-460">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-460">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="00039-461">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-461">Network</span></span>
* <span data-ttu-id="00039-462">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="00039-462">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="00039-463">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="00039-463">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="00039-464">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="00039-464">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="00039-465">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-465">Profile</span></span>
* <span data-ttu-id="00039-466">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="00039-466">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-467">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-467">RDBMS</span></span>
* <span data-ttu-id="00039-468">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="00039-468">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="00039-469">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-469">Resource</span></span>
* <span data-ttu-id="00039-470">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="00039-470">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="00039-471">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-471">Role</span></span>
* <span data-ttu-id="00039-472">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="00039-472">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="00039-473">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="00039-473">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="00039-474">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="00039-474">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="00039-475">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-475">Storage</span></span>
* <span data-ttu-id="00039-476">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="00039-476">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-477">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-477">VM</span></span>
* <span data-ttu-id="00039-478">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="00039-478">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="00039-479">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="00039-479">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="00039-480">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="00039-480">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="00039-481">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="00039-481">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="00039-482">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="00039-482">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="00039-483">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="00039-483">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="00039-484">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-484">October 23, 2018</span></span>

<span data-ttu-id="00039-485">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="00039-485">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="00039-486">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-486">Core</span></span>
* <span data-ttu-id="00039-487">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="00039-487">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="00039-488">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="00039-488">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="00039-489">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-489">ACR</span></span>
* <span data-ttu-id="00039-490">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="00039-490">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="00039-491">CDN</span><span class="sxs-lookup"><span data-stu-id="00039-491">CDN</span></span>
* <span data-ttu-id="00039-492">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="00039-492">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="00039-493">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="00039-493">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="00039-494">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-494">Container</span></span>
* <span data-ttu-id="00039-495">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="00039-495">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="00039-496">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-496">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="00039-497">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="00039-497">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="00039-498">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-498">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="00039-499">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="00039-499">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="00039-500">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="00039-500">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="00039-501">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="00039-501">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-502">CosmosDB</span></span>
* <span data-ttu-id="00039-503">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="00039-503">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-504">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-504">Interactive</span></span>
* <span data-ttu-id="00039-505">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="00039-505">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="00039-506">IoT Central</span><span class="sxs-lookup"><span data-stu-id="00039-506">IoT Central</span></span>
* <span data-ttu-id="00039-507">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="00039-507">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="00039-508">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="00039-508">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-509">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-509">Monitor</span></span>
* <span data-ttu-id="00039-510">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="00039-510">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="00039-511">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-511">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="00039-512">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="00039-512">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="00039-513">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="00039-513">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="00039-514">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="00039-514">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="00039-515">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="00039-515">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="00039-516">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="00039-516">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="00039-517">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="00039-517">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="00039-518">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="00039-518">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="00039-519">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="00039-519">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="00039-520">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-520">Network</span></span>
* <span data-ttu-id="00039-521">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="00039-521">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="00039-522">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="00039-522">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="00039-523">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="00039-523">ServiceBus</span></span>
* <span data-ttu-id="00039-524">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="00039-524">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="00039-525">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-525">SQL</span></span>
* <span data-ttu-id="00039-526">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="00039-526">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="00039-527">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-527">Storage</span></span>
* <span data-ttu-id="00039-528">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="00039-528">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="00039-529">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="00039-529">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="00039-530">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-530">VM</span></span>
* <span data-ttu-id="00039-531">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-531">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="00039-532">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-532">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="00039-533">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="00039-533">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="00039-534">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-534">October 16, 2018</span></span>

<span data-ttu-id="00039-535">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="00039-535">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="00039-536">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-536">VM</span></span>
* <span data-ttu-id="00039-537">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="00039-537">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="00039-538">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-538">October 9, 2018</span></span>

<span data-ttu-id="00039-539">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="00039-539">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="00039-540">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-540">Core</span></span>
* <span data-ttu-id="00039-541">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="00039-541">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="00039-542">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-542">ACR</span></span>
* <span data-ttu-id="00039-543">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="00039-543">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="00039-544">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-544">ACS</span></span>
* <span data-ttu-id="00039-545">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="00039-545">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="00039-546">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="00039-546">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="00039-547">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="00039-547">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="00039-548">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="00039-548">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="00039-549">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-549">Container</span></span>
* <span data-ttu-id="00039-550">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="00039-550">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="00039-551">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="00039-551">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="00039-552">Event Hub</span><span class="sxs-lookup"><span data-stu-id="00039-552">Event Hub</span></span>
* <span data-ttu-id="00039-553">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="00039-553">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="00039-554">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="00039-554">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="00039-555">Extensions</span><span class="sxs-lookup"><span data-stu-id="00039-555">Extensions</span></span>
* <span data-ttu-id="00039-556">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="00039-556">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="00039-557">HDInsight</span><span class="sxs-lookup"><span data-stu-id="00039-557">HDInsight</span></span>
* <span data-ttu-id="00039-558">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-558">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="00039-559">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-559">IoT</span></span>
* <span data-ttu-id="00039-560">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="00039-560">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-561">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-561">KeyVault</span></span>
* <span data-ttu-id="00039-562">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="00039-562">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="00039-563">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-563">Network</span></span>
* <span data-ttu-id="00039-564">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="00039-564">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="00039-565">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="00039-565">See #6052</span></span>
* <span data-ttu-id="00039-566">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="00039-566">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="00039-567">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="00039-567">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="00039-568">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="00039-568">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="00039-569">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="00039-569">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="00039-570">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="00039-570">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="00039-571">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="00039-571">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="00039-572">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-572">Role</span></span>
* <span data-ttu-id="00039-573">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="00039-573">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="00039-574">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="00039-574">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="00039-575">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="00039-575">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="00039-576">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="00039-576">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="00039-577">Service Bus</span><span class="sxs-lookup"><span data-stu-id="00039-577">Service Bus</span></span>
* <span data-ttu-id="00039-578">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="00039-578">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="00039-579">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-579">VM</span></span>
* <span data-ttu-id="00039-580">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="00039-580">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="00039-581">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="00039-581">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="00039-582">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="00039-582">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="00039-583">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="00039-583">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="00039-584">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="00039-584">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="00039-585">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="00039-585">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="00039-586">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="00039-586">September 21, 2018</span></span>

<span data-ttu-id="00039-587">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="00039-587">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="00039-588">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-588">ACR</span></span>
* <span data-ttu-id="00039-589">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="00039-589">Added ACR Task commands</span></span>
* <span data-ttu-id="00039-590">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="00039-590">Added quick run command</span></span>
* <span data-ttu-id="00039-591">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="00039-591">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="00039-592">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="00039-592">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="00039-593">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="00039-593">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="00039-594">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="00039-594">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="00039-595">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-595">ACS</span></span>
* <span data-ttu-id="00039-596">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="00039-596">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="00039-597">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="00039-597">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-598">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-598">AppService</span></span>

* <span data-ttu-id="00039-599">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="00039-599">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="00039-600">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="00039-600">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="00039-601">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="00039-601">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="00039-602">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="00039-602">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="00039-603">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-603">Batch</span></span>
* <span data-ttu-id="00039-604">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="00039-604">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="00039-605">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="00039-605">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="00039-606">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="00039-606">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="00039-607">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="00039-607">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00039-608">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-608">Batch AI</span></span> 
* <span data-ttu-id="00039-609">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="00039-609">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00039-610">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-610">Cognitive Services</span></span>
* <span data-ttu-id="00039-611">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="00039-611">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="00039-612">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="00039-612">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="00039-613">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="00039-613">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="00039-614">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="00039-614">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="00039-615">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="00039-615">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="00039-616">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="00039-616">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="00039-617">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-617">Container</span></span>
* <span data-ttu-id="00039-618">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="00039-618">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="00039-619">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="00039-619">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="00039-620">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="00039-620">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="00039-621">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-621">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="00039-622">DataLake</span><span class="sxs-lookup"><span data-stu-id="00039-622">Datalake</span></span>
* <span data-ttu-id="00039-623">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="00039-623">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="00039-624">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="00039-624">Interactive Shell</span></span>
* <span data-ttu-id="00039-625">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="00039-625">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="00039-626">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="00039-626">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="00039-627">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-627">IoT</span></span>
* <span data-ttu-id="00039-628">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="00039-628">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="00039-629">Key Vault</span><span class="sxs-lookup"><span data-stu-id="00039-629">Key Vault</span></span>
* <span data-ttu-id="00039-630">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="00039-630">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="00039-631">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-631">Network</span></span>
* <span data-ttu-id="00039-632">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="00039-632">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="00039-633">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="00039-633">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="00039-634">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="00039-634">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="00039-635">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="00039-635">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="00039-636">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="00039-636">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="00039-637">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="00039-637">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="00039-638">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="00039-638">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="00039-639">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="00039-639">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="00039-640">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="00039-640">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="00039-641">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="00039-641">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="00039-642">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="00039-642">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="00039-643">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="00039-643">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="00039-644">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="00039-644">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="00039-645">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="00039-645">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="00039-646">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="00039-646">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="00039-647">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="00039-647">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="00039-648">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="00039-648">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="00039-649">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="00039-649">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-650">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-650">RDBMS</span></span>
* <span data-ttu-id="00039-651">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="00039-651">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="00039-652">Réservation</span><span class="sxs-lookup"><span data-stu-id="00039-652">Reservation</span></span>
* <span data-ttu-id="00039-653">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="00039-653">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="00039-654">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="00039-654">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="00039-655">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="00039-655">Manage App</span></span>
* <span data-ttu-id="00039-656">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="00039-656">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="00039-657">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="00039-657">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="00039-658">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-658">Role</span></span>
* <span data-ttu-id="00039-659">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="00039-659">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="00039-660">SignalR</span><span class="sxs-lookup"><span data-stu-id="00039-660">SignalR</span></span>
* <span data-ttu-id="00039-661">Première version</span><span class="sxs-lookup"><span data-stu-id="00039-661">First release</span></span>

### <a name="storage"></a><span data-ttu-id="00039-662">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-662">Storage</span></span>
* <span data-ttu-id="00039-663">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="00039-663">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="00039-664">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="00039-664">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="00039-665">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-665">VM</span></span>
* <span data-ttu-id="00039-666">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="00039-666">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="00039-667">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="00039-667">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="00039-668">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="00039-668">August 28, 2018</span></span>

<span data-ttu-id="00039-669">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="00039-669">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="00039-670">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-670">Core</span></span>

* <span data-ttu-id="00039-671">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="00039-671">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="00039-672">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="00039-672">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="00039-673">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-673">ACR</span></span>

* <span data-ttu-id="00039-674">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="00039-674">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="00039-675">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="00039-675">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="00039-676">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-676">ACS</span></span>

* <span data-ttu-id="00039-677">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="00039-677">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="00039-678">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="00039-678">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-679">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-679">AppService</span></span>

* <span data-ttu-id="00039-680">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="00039-680">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="00039-681">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="00039-681">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="00039-682">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-682">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="00039-683">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="00039-683">Backup</span></span>

* <span data-ttu-id="00039-684">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-684">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="00039-685">Service de robot</span><span class="sxs-lookup"><span data-stu-id="00039-685">Bot Service</span></span>

* <span data-ttu-id="00039-686">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="00039-686">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00039-687">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-687">Cognitive Services</span></span>

* <span data-ttu-id="00039-688">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="00039-688">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="00039-689">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-689">IoT</span></span>

* <span data-ttu-id="00039-690">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="00039-690">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-691">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-691">Monitor</span></span>

* <span data-ttu-id="00039-692">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="00039-692">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="00039-693">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="00039-693">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="00039-694">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-694">Network</span></span>

* <span data-ttu-id="00039-695">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-695">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="00039-696">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-696">Resource</span></span>

* <span data-ttu-id="00039-697">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-697">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="00039-698">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-698">Storage</span></span>

* <span data-ttu-id="00039-699">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-699">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="00039-700">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-700">VM</span></span>

* <span data-ttu-id="00039-701">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-701">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="00039-702">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-702">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="00039-703">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="00039-703">Auguest 14, 2018</span></span>

<span data-ttu-id="00039-704">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="00039-704">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="00039-705">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-705">Core</span></span>

* <span data-ttu-id="00039-706">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="00039-706">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="00039-707">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="00039-707">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="00039-708">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="00039-708">Telemetry</span></span>

* <span data-ttu-id="00039-709">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="00039-709">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="00039-710">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-710">ACR</span></span>

* <span data-ttu-id="00039-711">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="00039-711">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="00039-712">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="00039-712">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="00039-713">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-713">ACS</span></span>

* <span data-ttu-id="00039-714">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="00039-714">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="00039-715">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="00039-715">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="00039-716">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="00039-716">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="00039-717">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="00039-717">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="00039-718">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="00039-718">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="00039-719">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-719">AppService</span></span>

* <span data-ttu-id="00039-720">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="00039-720">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="00039-721">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="00039-721">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="00039-722">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-722">BatchAI</span></span>

* <span data-ttu-id="00039-723">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="00039-723">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="00039-724">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-724">Container</span></span>

* <span data-ttu-id="00039-725">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-725">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="00039-726">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-726">IoT</span></span>

* <span data-ttu-id="00039-727">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="00039-727">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="00039-728">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="00039-728">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="00039-729">Iot Central</span><span class="sxs-lookup"><span data-stu-id="00039-729">Iot Central</span></span>

* <span data-ttu-id="00039-730">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="00039-730">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-731">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-731">KeyVault</span></span>


* <span data-ttu-id="00039-732">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="00039-732">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="00039-733">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="00039-733">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="00039-734">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="00039-734">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="00039-735">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="00039-735">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="00039-736">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="00039-736">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="00039-737">Relais</span><span class="sxs-lookup"><span data-stu-id="00039-737">Relay</span></span>

* <span data-ttu-id="00039-738">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-738">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="00039-739">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-739">Sql</span></span>

* <span data-ttu-id="00039-740">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="00039-740">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="00039-741">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-741">Storage</span></span>

* <span data-ttu-id="00039-742">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="00039-742">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="00039-743">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="00039-743">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="00039-744">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="00039-744">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="00039-745">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="00039-745">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="00039-746">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-746">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="00039-747">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-747">VM</span></span>

* <span data-ttu-id="00039-748">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="00039-748">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="00039-749">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="00039-749">July 31, 2018</span></span>

<span data-ttu-id="00039-750">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="00039-750">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="00039-751">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-751">ACR</span></span>

* <span data-ttu-id="00039-752">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="00039-752">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="00039-753">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="00039-753">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="00039-754">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-754">ACS</span></span>

* <span data-ttu-id="00039-755">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="00039-755">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="00039-756">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-756">Batch</span></span>

* <span data-ttu-id="00039-757">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00039-757">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="00039-758">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-758">Container</span></span>

* <span data-ttu-id="00039-759">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="00039-759">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="00039-760">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-760">Network</span></span>

* <span data-ttu-id="00039-761">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="00039-761">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="00039-762">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-762">Resource</span></span>

* <span data-ttu-id="00039-763">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="00039-763">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="00039-764">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="00039-764">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="00039-765">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-765">Role</span></span>

* <span data-ttu-id="00039-766">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="00039-766">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="00039-767">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="00039-767">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="00039-768">Recherche</span><span class="sxs-lookup"><span data-stu-id="00039-768">Search</span></span>

* <span data-ttu-id="00039-769">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="00039-769">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="00039-770">Service Bus</span><span class="sxs-lookup"><span data-stu-id="00039-770">Service Bus</span></span>

* <span data-ttu-id="00039-771">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="00039-771">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="00039-772">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-772">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="00039-773">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="00039-773">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="00039-774">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="00039-774">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-775">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-775">Storage</span></span>

* <span data-ttu-id="00039-776">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="00039-776">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="00039-777">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-777">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="00039-778">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-778">VM</span></span>

* <span data-ttu-id="00039-779">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-779">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="00039-780">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="00039-780">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="00039-781">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="00039-781">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="00039-782">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="00039-782">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="00039-783">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="00039-783">July 18, 2018</span></span>

<span data-ttu-id="00039-784">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="00039-784">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="00039-785">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-785">Core</span></span>

* <span data-ttu-id="00039-786">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="00039-786">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="00039-787">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="00039-787">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="00039-788">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="00039-788">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="00039-789">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-789">ACR</span></span>

* <span data-ttu-id="00039-790">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="00039-790">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="00039-791">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="00039-791">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="00039-792">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="00039-792">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="00039-793">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="00039-793">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="00039-794">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-794">ACS</span></span>

* <span data-ttu-id="00039-795">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="00039-795">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-796">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-796">AppService</span></span>

* <span data-ttu-id="00039-797">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="00039-797">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="00039-798">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-798">Batch</span></span>

* <span data-ttu-id="00039-799">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00039-799">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="00039-800">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="00039-800">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00039-801">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-801">Batch AI</span></span>

* <span data-ttu-id="00039-802">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="00039-802">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="00039-803">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-803">Container</span></span>

* <span data-ttu-id="00039-804">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="00039-804">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="00039-805">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="00039-805">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="00039-806">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-806">Network</span></span>

* <span data-ttu-id="00039-807">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="00039-807">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="00039-808">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="00039-808">Added `network nic wait`</span></span>
* <span data-ttu-id="00039-809">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="00039-809">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="00039-810">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="00039-810">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="00039-811">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-811">Resource</span></span>

* <span data-ttu-id="00039-812">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="00039-812">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="00039-813">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="00039-813">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="00039-814">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="00039-814">Added `deployment wait` command</span></span>
* <span data-ttu-id="00039-815">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="00039-815">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="00039-816">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-816">SQL</span></span>

* <span data-ttu-id="00039-817">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="00039-817">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="00039-818">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="00039-818">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="00039-819">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="00039-819">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="00039-820">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-820">Storage</span></span>

* <span data-ttu-id="00039-821">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="00039-821">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="00039-822">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-822">VM</span></span>

* <span data-ttu-id="00039-823">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-823">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="00039-824">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="00039-824">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="00039-825">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="00039-825">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="00039-826">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="00039-826">July 3, 2018</span></span>

<span data-ttu-id="00039-827">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="00039-827">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="00039-828">AKS</span><span class="sxs-lookup"><span data-stu-id="00039-828">AKS</span></span>

* <span data-ttu-id="00039-829">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-829">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="00039-830">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="00039-830">July 3, 2018</span></span>

<span data-ttu-id="00039-831">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="00039-831">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="00039-832">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-832">Core</span></span>

* <span data-ttu-id="00039-833">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="00039-833">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="00039-834">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-834">ACR</span></span>

* <span data-ttu-id="00039-835">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="00039-835">Added polling build status</span></span>
* <span data-ttu-id="00039-836">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="00039-836">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="00039-837">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="00039-837">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="00039-838">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-838">ACS</span></span>

* <span data-ttu-id="00039-839">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-839">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="00039-840">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-840">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="00039-841">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="00039-841">Updated options for `aks browse` command.</span></span> <span data-ttu-id="00039-842">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="00039-842">Added `--listen-port` support</span></span>
* <span data-ttu-id="00039-843">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="00039-843">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="00039-844">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="00039-844">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="00039-845">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="00039-845">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-846">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-846">AppService</span></span>

* <span data-ttu-id="00039-847">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="00039-847">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="00039-848">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="00039-848">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="00039-849">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="00039-849">Backup</span></span>

* <span data-ttu-id="00039-850">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="00039-850">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="00039-851">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-851">BatchAI</span></span>

* <span data-ttu-id="00039-852">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="00039-852">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="00039-853">Cloud</span><span class="sxs-lookup"><span data-stu-id="00039-853">Cloud</span></span>

* <span data-ttu-id="00039-854">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="00039-854">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="00039-855">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-855">Container</span></span>

* <span data-ttu-id="00039-856">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="00039-856">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="00039-857">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="00039-857">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="00039-858">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="00039-858">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="00039-859">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-859">Extension</span></span>

* <span data-ttu-id="00039-860">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="00039-860">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="00039-861">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-861">Network</span></span>

* <span data-ttu-id="00039-862">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="00039-862">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-863">Rdbms</span><span class="sxs-lookup"><span data-stu-id="00039-863">Rdbms</span></span>

* <span data-ttu-id="00039-864">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="00039-864">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="00039-865">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-865">Resource</span></span>

* <span data-ttu-id="00039-866">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="00039-866">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-867">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-867">VM</span></span>

* <span data-ttu-id="00039-868">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="00039-868">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="00039-869">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-869">June 25, 2018</span></span>

<span data-ttu-id="00039-870">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="00039-870">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="00039-871">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="00039-871">CLI</span></span>

* <span data-ttu-id="00039-872">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="00039-872">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="00039-873">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-873">June 19, 2018</span></span>

<span data-ttu-id="00039-874">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="00039-874">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="00039-875">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-875">Core</span></span>

* <span data-ttu-id="00039-876">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="00039-876">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="00039-877">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-877">ACR</span></span>

* <span data-ttu-id="00039-878">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="00039-878">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="00039-879">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="00039-879">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="00039-880">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-880">ACS</span></span>

* <span data-ttu-id="00039-881">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="00039-881">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="00039-882">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="00039-882">Added `--update` support</span></span>
* <span data-ttu-id="00039-883">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="00039-883">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="00039-884">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="00039-884">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="00039-885">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="00039-885">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="00039-886">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="00039-886">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="00039-887">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00039-887">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="00039-888">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00039-888">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-889">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-889">AppService</span></span>

* <span data-ttu-id="00039-890">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="00039-890">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="00039-891">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="00039-891">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="00039-892">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-892">Batch</span></span>

* <span data-ttu-id="00039-893">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="00039-893">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00039-894">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-894">Batch AI</span></span>

* <span data-ttu-id="00039-895">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="00039-895">Added support for workspaces.</span></span> <span data-ttu-id="00039-896">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="00039-896">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="00039-897">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="00039-897">Added support for experiments.</span></span> <span data-ttu-id="00039-898">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="00039-898">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="00039-899">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="00039-899">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="00039-900">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="00039-900">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="00039-901">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="00039-901">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="00039-902">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="00039-902">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="00039-903">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="00039-903">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="00039-904">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="00039-904">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="00039-905">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="00039-905">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="00039-906">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="00039-906">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="00039-907">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="00039-907">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="00039-908">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="00039-908">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="00039-909">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="00039-909">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="00039-910">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="00039-910">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="00039-911">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="00039-911">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="00039-912">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="00039-912">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="00039-913">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="00039-913">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="00039-914">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="00039-914">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="00039-915">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="00039-915">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="00039-916">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="00039-916">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="00039-917">Cartes</span><span class="sxs-lookup"><span data-stu-id="00039-917">Maps</span></span>

* <span data-ttu-id="00039-918">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="00039-918">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="00039-919">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-919">Network</span></span>

* <span data-ttu-id="00039-920">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="00039-920">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="00039-921">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="00039-921">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="00039-922">#6502</span><span class="sxs-lookup"><span data-stu-id="00039-922">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="00039-923">Réservations</span><span class="sxs-lookup"><span data-stu-id="00039-923">Reservations</span></span>

* <span data-ttu-id="00039-924">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="00039-924">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="00039-925">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="00039-925">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="00039-926">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="00039-926">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="00039-927">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="00039-927">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="00039-928">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="00039-928">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="00039-929">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="00039-929">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="00039-930">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-930">Role</span></span>

* <span data-ttu-id="00039-931">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="00039-931">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="00039-932">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-932">SQL</span></span>

* <span data-ttu-id="00039-933">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-933">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="00039-934">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-934">Storage</span></span>

* <span data-ttu-id="00039-935">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="00039-935">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="00039-936">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-936">VM</span></span>

* <span data-ttu-id="00039-937">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-937">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="00039-938">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="00039-938">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="00039-939">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="00039-939">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="00039-940">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-940">June 13, 2018</span></span>

<span data-ttu-id="00039-941">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="00039-941">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="00039-942">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-942">Core</span></span>

* <span data-ttu-id="00039-943">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="00039-943">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="00039-944">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-944">June 13, 2018</span></span>

<span data-ttu-id="00039-945">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="00039-945">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="00039-946">AKS</span><span class="sxs-lookup"><span data-stu-id="00039-946">AKS</span></span>

* <span data-ttu-id="00039-947">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-947">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="00039-948">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="00039-948">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="00039-949">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-949">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="00039-950">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-950">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="00039-951">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-951">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-952">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-952">AppService</span></span>

* <span data-ttu-id="00039-953">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="00039-953">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="00039-954">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-954">June 5, 2018</span></span>

<span data-ttu-id="00039-955">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="00039-955">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-956">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-956">Interactive</span></span>

* <span data-ttu-id="00039-957">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="00039-957">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="00039-958">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="00039-958">June 5, 2018</span></span>

<span data-ttu-id="00039-959">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="00039-959">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="00039-960">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-960">Core</span></span>

* <span data-ttu-id="00039-961">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="00039-961">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="00039-962">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="00039-962">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="00039-963">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-963">ACR</span></span>

* <span data-ttu-id="00039-964">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="00039-964">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="00039-965">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="00039-965">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="00039-966">AKS</span><span class="sxs-lookup"><span data-stu-id="00039-966">AKS</span></span>

* <span data-ttu-id="00039-967">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="00039-967">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="00039-968">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-968">Batch</span></span>

* <span data-ttu-id="00039-969">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="00039-969">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="00039-970">IOT</span><span class="sxs-lookup"><span data-stu-id="00039-970">IOT</span></span>

* <span data-ttu-id="00039-971">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="00039-971">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="00039-972">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-972">Network</span></span>

* <span data-ttu-id="00039-973">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="00039-973">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="00039-974">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="00039-974">Policy Insights</span></span>

* <span data-ttu-id="00039-975">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-975">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="00039-976">ARM</span><span class="sxs-lookup"><span data-stu-id="00039-976">ARM</span></span>

* <span data-ttu-id="00039-977">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="00039-977">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="00039-978">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-978">SQL</span></span>

* <span data-ttu-id="00039-979">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="00039-979">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="00039-980">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="00039-980">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="00039-981">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-981">Storage</span></span>

* <span data-ttu-id="00039-982">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="00039-982">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="00039-983">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-983">VM</span></span>

* <span data-ttu-id="00039-984">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="00039-984">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="00039-985">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-985">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="00039-986">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="00039-986">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="00039-987">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="00039-987">May 22, 2018</span></span>

<span data-ttu-id="00039-988">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="00039-988">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="00039-989">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-989">Core</span></span>

* <span data-ttu-id="00039-990">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="00039-990">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="00039-991">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-991">ACS</span></span>

* <span data-ttu-id="00039-992">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="00039-992">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="00039-993">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="00039-993">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-994">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-994">AppService</span></span>

* <span data-ttu-id="00039-995">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="00039-995">Improved generic update commands</span></span>
* <span data-ttu-id="00039-996">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="00039-996">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="00039-997">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-997">Container</span></span>

* <span data-ttu-id="00039-998">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="00039-998">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="00039-999">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-999">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1000">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1000">Extension</span></span>

* <span data-ttu-id="00039-1001">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="00039-1001">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1002">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1002">Interactive</span></span>

* <span data-ttu-id="00039-1003">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="00039-1003">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="00039-1004">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="00039-1004">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-1005">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-1005">KeyVault</span></span>

* <span data-ttu-id="00039-1006">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="00039-1006">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="00039-1007">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1007">Network</span></span>

* <span data-ttu-id="00039-1008">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="00039-1008">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="00039-1009">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="00039-1009">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1010">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1010">SQL</span></span>

* <span data-ttu-id="00039-1011">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="00039-1011">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="00039-1012">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="00039-1012">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="00039-1013">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="00039-1013">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="00039-1014">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="00039-1014">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="00039-1015">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="00039-1015">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="00039-1016">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="00039-1016">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="00039-1017">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="00039-1017">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="00039-1018">`edition`.</span><span class="sxs-lookup"><span data-stu-id="00039-1018">`edition`.</span></span> <span data-ttu-id="00039-1019">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="00039-1019">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="00039-1020">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="00039-1020">`elasticPoolName`.</span></span> <span data-ttu-id="00039-1021">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="00039-1021">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="00039-1022">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="00039-1022">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="00039-1023">`edition`.</span><span class="sxs-lookup"><span data-stu-id="00039-1023">`edition`.</span></span> <span data-ttu-id="00039-1024">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="00039-1024">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="00039-1025">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="00039-1025">`dtu`.</span></span> <span data-ttu-id="00039-1026">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="00039-1026">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="00039-1027">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="00039-1027">`databaseDtuMin`.</span></span> <span data-ttu-id="00039-1028">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="00039-1028">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="00039-1029">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="00039-1029">`databaseDtuMax`.</span></span> <span data-ttu-id="00039-1030">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="00039-1030">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="00039-1031">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="00039-1031">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="00039-1032">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="00039-1032">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1033">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1033">Storage</span></span>

* <span data-ttu-id="00039-1034">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="00039-1034">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="00039-1035">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="00039-1035">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1036">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1036">VM</span></span>

* <span data-ttu-id="00039-1037">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="00039-1037">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="00039-1038">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="00039-1038">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="00039-1039">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="00039-1039">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="00039-1040">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="00039-1040">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="00039-1041">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="00039-1041">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="00039-1042">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1042">May 7, 2018</span></span>

<span data-ttu-id="00039-1043">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="00039-1043">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="00039-1044">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1044">Core</span></span>

* <span data-ttu-id="00039-1045">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="00039-1045">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="00039-1046">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="00039-1046">Added limited support for positional arguments</span></span>
* <span data-ttu-id="00039-1047">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="00039-1047">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="00039-1048">#5591</span><span class="sxs-lookup"><span data-stu-id="00039-1048">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="00039-1049">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="00039-1049">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="00039-1050">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="00039-1050">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="00039-1051">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="00039-1051">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="00039-1052">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="00039-1052">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="00039-1053">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="00039-1053">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1054">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1054">ACR</span></span>

* <span data-ttu-id="00039-1055">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1055">Added ACR Build commands</span></span>
* <span data-ttu-id="00039-1056">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="00039-1056">Improved resource not found error messages</span></span>
* <span data-ttu-id="00039-1057">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="00039-1057">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="00039-1058">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="00039-1058">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="00039-1059">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="00039-1059">Improved repository commands error messages</span></span>
* <span data-ttu-id="00039-1060">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="00039-1060">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1061">ACS</span></span>

* <span data-ttu-id="00039-1062">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="00039-1062">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="00039-1063">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="00039-1063">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="00039-1064">AMS</span><span class="sxs-lookup"><span data-stu-id="00039-1064">AMS</span></span>

* <span data-ttu-id="00039-1065">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="00039-1065">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1066">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1066">Appservice</span></span>

* <span data-ttu-id="00039-1067">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="00039-1067">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="00039-1068">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="00039-1068">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="00039-1069">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="00039-1069">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="00039-1070">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-1070">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00039-1071">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-1071">Batch AI</span></span>

* <span data-ttu-id="00039-1072">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="00039-1072">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00039-1073">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-1073">Cognitive Services</span></span>

* <span data-ttu-id="00039-1074">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="00039-1074">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-1075">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1075">Consumption</span></span>

* <span data-ttu-id="00039-1076">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="00039-1076">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="00039-1077">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1077">Container</span></span>

* <span data-ttu-id="00039-1078">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="00039-1078">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="00039-1079">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="00039-1079">Cosmos DB</span></span>

* <span data-ttu-id="00039-1080">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="00039-1080">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="00039-1081">DMS</span><span class="sxs-lookup"><span data-stu-id="00039-1081">DMS</span></span>

* <span data-ttu-id="00039-1082">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="00039-1082">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1083">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1083">Extension</span></span>

* <span data-ttu-id="00039-1084">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="00039-1084">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1085">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1085">Interactive</span></span>

* <span data-ttu-id="00039-1086">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="00039-1086">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="00039-1087">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="00039-1087">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="00039-1088">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="00039-1088">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="00039-1089">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="00039-1089">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="00039-1090">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-1090">Lab</span></span>

* <span data-ttu-id="00039-1091">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="00039-1091">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="00039-1092">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1092">Network</span></span>

* <span data-ttu-id="00039-1093">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="00039-1093">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="00039-1094">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1094">Profile</span></span>

* <span data-ttu-id="00039-1095">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="00039-1095">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="00039-1096">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="00039-1096">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="00039-1097">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="00039-1097">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="00039-1098">Redis</span><span class="sxs-lookup"><span data-stu-id="00039-1098">Redis</span></span>

* <span data-ttu-id="00039-1099">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="00039-1099">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="00039-1100">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="00039-1100">Deprecated `redis list-all`.</span></span> <span data-ttu-id="00039-1101">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="00039-1101">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="00039-1102">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="00039-1102">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="00039-1103">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="00039-1103">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="00039-1104">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1104">Role</span></span>

* <span data-ttu-id="00039-1105">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="00039-1105">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1106">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1106">Storage</span></span>

* <span data-ttu-id="00039-1107">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="00039-1107">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="00039-1108">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="00039-1108">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="00039-1109">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="00039-1109">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="00039-1110">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="00039-1110">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="00039-1111">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="00039-1111">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1112">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1112">VM</span></span>

* <span data-ttu-id="00039-1113">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="00039-1113">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="00039-1114">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="00039-1114">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="00039-1115">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="00039-1115">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="00039-1116">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="00039-1116">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="00039-1117">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="00039-1117">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="00039-1118">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="00039-1118">Added write accelerator support</span></span>
* <span data-ttu-id="00039-1119">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="00039-1119">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="00039-1120">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1120">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="00039-1121">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="00039-1121">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="00039-1122">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1122">April 10, 2018</span></span>

<span data-ttu-id="00039-1123">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="00039-1123">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1124">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1124">ACR</span></span>

* <span data-ttu-id="00039-1125">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="00039-1125">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1126">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1126">ACS</span></span>

* <span data-ttu-id="00039-1127">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="00039-1127">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1128">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="00039-1130">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="00039-1130">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="00039-1131">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-1131">BatchAI</span></span>

* <span data-ttu-id="00039-1132">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="00039-1132">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="00039-1133">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="00039-1133">Job level mounting</span></span>
  - <span data-ttu-id="00039-1134">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="00039-1134">Environment variables with secret values</span></span>
  - <span data-ttu-id="00039-1135">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="00039-1135">Performance counters settings</span></span>
  - <span data-ttu-id="00039-1136">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="00039-1136">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="00039-1137">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="00039-1137">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="00039-1138">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="00039-1138">Usage and limits reporting</span></span>
  - <span data-ttu-id="00039-1139">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="00039-1139">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="00039-1140">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="00039-1140">Support for custom images</span></span>
  - <span data-ttu-id="00039-1141">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="00039-1141">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="00039-1142">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="00039-1142">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="00039-1143">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="00039-1143">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="00039-1144">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="00039-1144">National clouds are supported</span></span>
* <span data-ttu-id="00039-1145">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="00039-1145">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="00039-1146">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="00039-1146">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="00039-1147">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-1147">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="00039-1148">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="00039-1148">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="00039-1149">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="00039-1149">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="00039-1150">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="00039-1150">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="00039-1151">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="00039-1151">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="00039-1152">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="00039-1152">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="00039-1153">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="00039-1153">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="00039-1154">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="00039-1154">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="00039-1155">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="00039-1155">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="00039-1156">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="00039-1156">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="00039-1157">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="00039-1157">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="00039-1158">Facturation</span><span class="sxs-lookup"><span data-stu-id="00039-1158">Billing</span></span>

* <span data-ttu-id="00039-1159">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="00039-1159">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-1160">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1160">Consumption</span></span>

* <span data-ttu-id="00039-1161">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="00039-1161">Added `marketplace` commands</span></span>
* <span data-ttu-id="00039-1162">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="00039-1162">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="00039-1163">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="00039-1163">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="00039-1164">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="00039-1164">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="00039-1165">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="00039-1165">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="00039-1166">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="00039-1166">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="00039-1167">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1167">Container</span></span>

* <span data-ttu-id="00039-1168">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="00039-1168">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="00039-1169">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="00039-1169">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1170">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1170">Extension</span></span>

* <span data-ttu-id="00039-1171">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="00039-1171">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1172">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1172">Interactive</span></span>

* <span data-ttu-id="00039-1173">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="00039-1173">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="00039-1174">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="00039-1174">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="00039-1175">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="00039-1175">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="00039-1176">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1176">Network</span></span>

* <span data-ttu-id="00039-1177">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="00039-1177">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="00039-1178">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="00039-1178">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="00039-1179">#4910</span><span class="sxs-lookup"><span data-stu-id="00039-1179">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="00039-1180">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="00039-1180">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="00039-1181">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="00039-1181">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="00039-1182">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1182">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="00039-1183">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1183">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="00039-1184">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="00039-1184">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1185">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1185">Profile</span></span>

* <span data-ttu-id="00039-1186">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="00039-1186">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="00039-1187">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="00039-1187">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-1188">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-1188">RDBMS</span></span>

* <span data-ttu-id="00039-1189">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="00039-1189">Added `georestore` command</span></span>
* <span data-ttu-id="00039-1190">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="00039-1190">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1191">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1191">Resource</span></span>

* <span data-ttu-id="00039-1192">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="00039-1192">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="00039-1193">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="00039-1193">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1194">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1194">SQL</span></span>

* <span data-ttu-id="00039-1195">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="00039-1195">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1196">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1196">Storage</span></span>

* <span data-ttu-id="00039-1197">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="00039-1197">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1198">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1198">VM</span></span>

* <span data-ttu-id="00039-1199">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00039-1199">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="00039-1200">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="00039-1200">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="00039-1202">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-1202">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="00039-1203">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="00039-1203">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="00039-1204">#5718</span><span class="sxs-lookup"><span data-stu-id="00039-1204">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="00039-1205">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="00039-1205">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="00039-1206">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1206">March 27, 2018</span></span>

<span data-ttu-id="00039-1207">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="00039-1207">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="00039-1208">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1208">Core</span></span>

* <span data-ttu-id="00039-1209">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="00039-1209">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1210">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1210">ACS</span></span>

* <span data-ttu-id="00039-1211">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00039-1211">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1212">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1212">Appservice</span></span>

* <span data-ttu-id="00039-1213">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="00039-1213">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="00039-1214">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-1214">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="00039-1215">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="00039-1215">Backup</span></span>

* <span data-ttu-id="00039-1216">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="00039-1216">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="00039-1217">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-1217">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="00039-1218">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="00039-1218">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="00039-1219">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="00039-1219">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="00039-1220">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1220">Container</span></span>

* <span data-ttu-id="00039-1221">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="00039-1221">Added `container exec` command.</span></span> <span data-ttu-id="00039-1222">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="00039-1222">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="00039-1223">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-1223">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1224">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1224">Extension</span></span>

* <span data-ttu-id="00039-1225">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="00039-1225">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="00039-1226">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="00039-1226">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="00039-1227">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1227">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1228">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1228">Interactive</span></span>

* <span data-ttu-id="00039-1229">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="00039-1229">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="00039-1230">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="00039-1230">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="00039-1231">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="00039-1231">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="00039-1232">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="00039-1232">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="00039-1233">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-1233">Lab</span></span>

* <span data-ttu-id="00039-1234">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="00039-1234">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1235">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1235">Monitor</span></span>

* <span data-ttu-id="00039-1236">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="00039-1236">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="00039-1237">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="00039-1237">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="00039-1238">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="00039-1238">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="00039-1239">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1239">Network</span></span>

* <span data-ttu-id="00039-1240">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="00039-1240">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1241">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1241">Profile</span></span>

* <span data-ttu-id="00039-1242">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="00039-1242">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-1243">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-1243">RDBMS</span></span>

* <span data-ttu-id="00039-1244">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="00039-1244">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1245">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1245">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="00039-1247">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1247">Role</span></span>

* <span data-ttu-id="00039-1248">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="00039-1248">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="00039-1249">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="00039-1249">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="00039-1250">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="00039-1250">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="00039-1251">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-1251">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="00039-1252">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="00039-1252">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1253">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1253">Storage</span></span>

* <span data-ttu-id="00039-1254">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="00039-1254">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="00039-1255">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="00039-1255">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1256">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1256">VM</span></span>

* <span data-ttu-id="00039-1257">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="00039-1257">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="00039-1258">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="00039-1258">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="00039-1259">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="00039-1259">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="00039-1260">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="00039-1260">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="00039-1261">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1261">March 13, 2018</span></span>

<span data-ttu-id="00039-1262">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="00039-1262">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1263">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1263">ACR</span></span>

* <span data-ttu-id="00039-1264">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="00039-1264">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="00039-1265">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="00039-1265">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="00039-1266">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="00039-1266">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1267">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1267">ACS</span></span>

* <span data-ttu-id="00039-1268">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="00039-1268">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="00039-1269">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="00039-1269">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="00039-1270">Advisor</span><span class="sxs-lookup"><span data-stu-id="00039-1270">Advisor</span></span>

* <span data-ttu-id="00039-1271">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="00039-1271">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="00039-1272">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="00039-1272">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="00039-1273">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="00039-1273">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="00039-1274">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="00039-1274">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="00039-1275">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="00039-1275">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1276">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1276">Appservice</span></span>

* <span data-ttu-id="00039-1277">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="00039-1277">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="00039-1278">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-1278">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="00039-1279">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="00039-1279">Eventhubs</span></span>

* <span data-ttu-id="00039-1280">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1280">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1281">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1281">Extension</span></span>

* <span data-ttu-id="00039-1282">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="00039-1282">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1283">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1283">Interactive</span></span>

* <span data-ttu-id="00039-1284">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="00039-1284">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="00039-1285">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="00039-1285">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="00039-1286">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="00039-1286">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="00039-1287">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="00039-1287">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1288">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1288">Monitor</span></span>

* <span data-ttu-id="00039-1289">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="00039-1289">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="00039-1290">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="00039-1290">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="00039-1291">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="00039-1291">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="00039-1292">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="00039-1292">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="00039-1293">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1293">Network</span></span>

* <span data-ttu-id="00039-1294">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="00039-1294">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="00039-1295">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="00039-1295">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="00039-1296">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="00039-1296">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="00039-1297">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="00039-1297">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1298">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1298">Profile</span></span>

* <span data-ttu-id="00039-1299">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="00039-1299">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="00039-1300">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="00039-1300">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-1301">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-1301">RDBMS</span></span>

* <span data-ttu-id="00039-1302">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="00039-1302">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="00039-1303">Service Bus</span><span class="sxs-lookup"><span data-stu-id="00039-1303">Service Bus</span></span>

* <span data-ttu-id="00039-1304">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1304">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1305">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1305">Storage</span></span>

* <span data-ttu-id="00039-1306">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="00039-1306">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="00039-1307">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="00039-1307">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1308">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1308">VM</span></span>

* <span data-ttu-id="00039-1309">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="00039-1309">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="00039-1310">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="00039-1310">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="00039-1311">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="00039-1311">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="00039-1312">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="00039-1312">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="00039-1313">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1313">February 27, 2018</span></span>

<span data-ttu-id="00039-1314">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="00039-1314">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="00039-1315">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1315">Core</span></span>

* <span data-ttu-id="00039-1316">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="00039-1316">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="00039-1317">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="00039-1317">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="00039-1318">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="00039-1318">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1319">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1319">ACS</span></span>

* <span data-ttu-id="00039-1320">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1320">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="00039-1321">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="00039-1321">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="00039-1322">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00039-1322">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="00039-1323">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="00039-1323">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1324">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1324">Appservice</span></span>

* <span data-ttu-id="00039-1325">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="00039-1325">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="00039-1326">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="00039-1326">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00039-1327">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-1327">Cognitive Services</span></span>

* <span data-ttu-id="00039-1328">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-1328">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-1329">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1329">Consumption</span></span>

* <span data-ttu-id="00039-1330">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="00039-1330">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="00039-1331">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="00039-1331">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="00039-1332">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1332">Container</span></span>

* <span data-ttu-id="00039-1333">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="00039-1333">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="00039-1334">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1334">Network</span></span>

* <span data-ttu-id="00039-1335">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="00039-1335">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1336">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1336">Resource</span></span>

* <span data-ttu-id="00039-1337">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="00039-1337">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="00039-1338">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1338">Role</span></span>

* <span data-ttu-id="00039-1339">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="00039-1339">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1340">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1340">SQL</span></span>

* <span data-ttu-id="00039-1341">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="00039-1341">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1342">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1342">Storage</span></span>

* <span data-ttu-id="00039-1343">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="00039-1343">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1344">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1344">VM</span></span>

* <span data-ttu-id="00039-1345">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="00039-1345">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="00039-1346">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1346">February 13, 2018</span></span>

<span data-ttu-id="00039-1347">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="00039-1347">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="00039-1348">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1348">Core</span></span>

* <span data-ttu-id="00039-1349">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="00039-1349">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1350">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1350">ACS</span></span>

* <span data-ttu-id="00039-1351">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="00039-1351">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="00039-1352">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="00039-1352">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="00039-1353">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00039-1353">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="00039-1354">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="00039-1354">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="00039-1355">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="00039-1355">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="00039-1356">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="00039-1356">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="00039-1357">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00039-1357">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="00039-1358">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="00039-1358">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1359">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1359">Appservice</span></span>

* <span data-ttu-id="00039-1360">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="00039-1360">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="00039-1361">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="00039-1361">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="00039-1362">CDN</span><span class="sxs-lookup"><span data-stu-id="00039-1362">CDN</span></span>

* <span data-ttu-id="00039-1363">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="00039-1363">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="00039-1364">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1364">Container</span></span>

* <span data-ttu-id="00039-1365">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="00039-1365">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="00039-1366">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1366">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-1367">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-1367">CosmosDB</span></span>

* <span data-ttu-id="00039-1368">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="00039-1368">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1369">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1369">Extension</span></span>

* <span data-ttu-id="00039-1370">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1370">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="00039-1371">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1371">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="00039-1372">Commentaires</span><span class="sxs-lookup"><span data-stu-id="00039-1372">Feedback</span></span>

* <span data-ttu-id="00039-1373">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="00039-1373">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1374">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1374">Interactive</span></span>

* <span data-ttu-id="00039-1375">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00039-1375">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="00039-1376">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="00039-1376">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="00039-1377">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1377">IoT</span></span>

* <span data-ttu-id="00039-1378">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="00039-1378">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="00039-1379">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="00039-1379">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="00039-1380">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1380">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="00039-1381">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="00039-1381">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1382">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1382">Monitor</span></span>

* <span data-ttu-id="00039-1383">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="00039-1383">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="00039-1384">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1384">Network</span></span>

* <span data-ttu-id="00039-1385">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="00039-1385">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="00039-1386">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1386">Profile</span></span>

* <span data-ttu-id="00039-1387">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="00039-1387">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1388">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1388">Resource</span></span>

* <span data-ttu-id="00039-1389">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="00039-1389">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="00039-1390">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1390">Role</span></span>

* <span data-ttu-id="00039-1391">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="00039-1391">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1392">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1392">SQL</span></span>

* <span data-ttu-id="00039-1393">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="00039-1393">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="00039-1394">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="00039-1394">Added `sql db rename`</span></span>
* <span data-ttu-id="00039-1395">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="00039-1395">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1396">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1396">Storage</span></span>

* <span data-ttu-id="00039-1397">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="00039-1397">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1398">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1398">VM</span></span>

* <span data-ttu-id="00039-1399">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="00039-1399">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="00039-1400">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="00039-1400">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="00039-1401">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="00039-1401">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="00039-1402">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1402">January 31, 2018</span></span>

<span data-ttu-id="00039-1403">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="00039-1403">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="00039-1404">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1404">Core</span></span>

* <span data-ttu-id="00039-1405">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="00039-1405">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="00039-1406">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="00039-1406">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="00039-1407">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="00039-1407">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="00039-1408">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="00039-1408">Use `--verbose` to see</span></span>
* <span data-ttu-id="00039-1409">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="00039-1409">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1410">ACS</span></span>

* <span data-ttu-id="00039-1411">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="00039-1411">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="00039-1412">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="00039-1412">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1413">Appservice</span></span>

* <span data-ttu-id="00039-1414">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="00039-1414">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="00039-1415">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="00039-1415">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="00039-1416">CDN</span><span class="sxs-lookup"><span data-stu-id="00039-1416">CDN</span></span>

* <span data-ttu-id="00039-1417">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="00039-1417">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-1418">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-1418">CosmosDB</span></span>

* <span data-ttu-id="00039-1419">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="00039-1419">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1420">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1420">Interactive</span></span>

* <span data-ttu-id="00039-1421">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="00039-1421">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="00039-1422">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1422">Network</span></span>

* <span data-ttu-id="00039-1423">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="00039-1423">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="00039-1424">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1424">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="00039-1425">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="00039-1425">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="00039-1426">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="00039-1426">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="00039-1427">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="00039-1427">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="00039-1428">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="00039-1428">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="00039-1429">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="00039-1429">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="00039-1430">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="00039-1430">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="00039-1431">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="00039-1431">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="00039-1432">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="00039-1432">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1433">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1433">Profile</span></span>

* <span data-ttu-id="00039-1434">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="00039-1434">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1435">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1435">Resource</span></span>

* <span data-ttu-id="00039-1436">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="00039-1436">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1437">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1437">Storage</span></span>

* <span data-ttu-id="00039-1438">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="00039-1438">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="00039-1439">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="00039-1439">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="00039-1440">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="00039-1440">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="00039-1441">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-1441">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="00039-1442">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="00039-1442">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1443">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1443">VM</span></span>

* <span data-ttu-id="00039-1444">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="00039-1444">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="00039-1445">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="00039-1445">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="00039-1446">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="00039-1446">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="00039-1447">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1447">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="00039-1448">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="00039-1448">January 17, 2018</span></span>

<span data-ttu-id="00039-1449">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="00039-1449">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1450">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1450">ACR</span></span>

* <span data-ttu-id="00039-1451">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="00039-1451">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="00039-1452">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="00039-1452">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1453">ACS</span></span>

* <span data-ttu-id="00039-1454">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="00039-1454">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="00039-1455">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="00039-1455">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1456">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1456">Appservice</span></span>

* <span data-ttu-id="00039-1457">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="00039-1457">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="00039-1458">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="00039-1458">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="00039-1459">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="00039-1459">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="00039-1460">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="00039-1460">Backup</span></span>

* <span data-ttu-id="00039-1461">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="00039-1461">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="00039-1462">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="00039-1462">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="00039-1463">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="00039-1463">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="00039-1464">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="00039-1464">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="00039-1465">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1465">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="00039-1466">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1466">Batch</span></span>

* <span data-ttu-id="00039-1467">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="00039-1467">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="00039-1468">Cloud</span><span class="sxs-lookup"><span data-stu-id="00039-1468">Cloud</span></span>

* <span data-ttu-id="00039-1469">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="00039-1469">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-1470">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1470">Consumption</span></span>

* <span data-ttu-id="00039-1471">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="00039-1471">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="00039-1472">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00039-1472">Event Grid</span></span>

* <span data-ttu-id="00039-1473">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="00039-1473">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="00039-1474">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="00039-1474">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="00039-1475">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="00039-1475">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="00039-1476">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="00039-1476">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="00039-1477">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="00039-1477">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="00039-1478">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="00039-1478">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="00039-1479">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="00039-1479">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="00039-1480">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="00039-1480">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1481">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1481">Interactive</span></span>

* <span data-ttu-id="00039-1482">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="00039-1482">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="00039-1483">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="00039-1483">Fixed errors on startup</span></span>
* <span data-ttu-id="00039-1484">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="00039-1484">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="00039-1485">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1485">IoT</span></span>

* <span data-ttu-id="00039-1486">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="00039-1486">Added support for device provisioning service</span></span>
* <span data-ttu-id="00039-1487">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="00039-1487">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="00039-1488">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1488">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1489">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1489">Monitor</span></span>

* <span data-ttu-id="00039-1490">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="00039-1490">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="00039-1491">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="00039-1491">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="00039-1492">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="00039-1492">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="00039-1493">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1493">Network</span></span>

* <span data-ttu-id="00039-1494">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="00039-1494">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="00039-1495">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1495">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1496">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1496">Profile</span></span>

* <span data-ttu-id="00039-1497">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="00039-1497">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="00039-1498">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1498">Role</span></span>

* <span data-ttu-id="00039-1499">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="00039-1499">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00039-1500">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00039-1500">Service Fabric</span></span>

* <span data-ttu-id="00039-1501">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="00039-1501">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="00039-1502">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="00039-1502">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1503">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1503">VM</span></span>

* <span data-ttu-id="00039-1504">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="00039-1504">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="00039-1505">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="00039-1505">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="00039-1506">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="00039-1506">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="00039-1507">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="00039-1507">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="00039-1508">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="00039-1508">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="00039-1509">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1509">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="00039-1510">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1510">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="00039-1511">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="00039-1511">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="00039-1512">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1512">December 19, 2017</span></span>

<span data-ttu-id="00039-1513">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="00039-1513">Version 2.0.23</span></span>

* <span data-ttu-id="00039-1514">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="00039-1514">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="00039-1515">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1515">Container</span></span>

* <span data-ttu-id="00039-1516">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1516">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="00039-1517">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1517">Network</span></span>

* <span data-ttu-id="00039-1518">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1518">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="00039-1519">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1519">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1520">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1520">Storage</span></span>

* <span data-ttu-id="00039-1521">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="00039-1521">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1522">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1522">VM</span></span>

* <span data-ttu-id="00039-1523">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="00039-1523">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="00039-1524">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1524">December 5, 2017</span></span>

<span data-ttu-id="00039-1525">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="00039-1525">Version 2.0.22</span></span>

* <span data-ttu-id="00039-1526">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="00039-1526">Removed `az component` commands.</span></span> <span data-ttu-id="00039-1527">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="00039-1527">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="00039-1528">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1528">Core</span></span>
* <span data-ttu-id="00039-1529">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="00039-1529">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="00039-1530">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="00039-1530">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1531">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1531">ACS</span></span>

* <span data-ttu-id="00039-1532">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="00039-1532">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="00039-1533">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="00039-1533">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="00039-1534">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="00039-1534">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="00039-1535">Advisor</span><span class="sxs-lookup"><span data-stu-id="00039-1535">Advisor</span></span>

* <span data-ttu-id="00039-1536">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1536">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1537">Appservice</span></span>

* <span data-ttu-id="00039-1538">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="00039-1538">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="00039-1539">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="00039-1539">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="00039-1540">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="00039-1540">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="00039-1541">Consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1541">Consumption</span></span>

* <span data-ttu-id="00039-1542">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="00039-1542">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="00039-1543">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1543">Container</span></span>

* <span data-ttu-id="00039-1544">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1544">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1545">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1545">Monitor</span></span>

* <span data-ttu-id="00039-1546">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="00039-1546">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1547">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1547">Resource</span></span>

* <span data-ttu-id="00039-1548">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="00039-1548">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="00039-1549">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1549">Role</span></span>

* <span data-ttu-id="00039-1550">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="00039-1550">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="00039-1551">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="00039-1551">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="00039-1552">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="00039-1552">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1553">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1553">SQL</span></span>

* <span data-ttu-id="00039-1554">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="00039-1554">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="00039-1555">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="00039-1555">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1556">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1556">VM</span></span>

* <span data-ttu-id="00039-1557">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="00039-1557">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="00039-1558">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1558">November 14, 2017</span></span>

<span data-ttu-id="00039-1559">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="00039-1559">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1560">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1560">ACR</span></span>

* <span data-ttu-id="00039-1561">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="00039-1561">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="00039-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1562">ACS</span></span>

* <span data-ttu-id="00039-1563">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="00039-1563">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="00039-1564">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="00039-1564">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="00039-1565">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="00039-1565">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="00039-1566">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="00039-1566">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="00039-1567">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="00039-1567">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1568">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1568">Appservice</span></span>

* <span data-ttu-id="00039-1569">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="00039-1569">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="00039-1570">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="00039-1570">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="00039-1571">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="00039-1571">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="00039-1572">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="00039-1572">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="00039-1573">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="00039-1573">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="00039-1574">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="00039-1574">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="00039-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1575">Batch</span></span>

* <span data-ttu-id="00039-1576">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="00039-1576">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="00039-1577">Batchai</span><span class="sxs-lookup"><span data-stu-id="00039-1577">Batchai</span></span>

* <span data-ttu-id="00039-1578">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="00039-1578">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="00039-1579">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="00039-1579">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="00039-1580">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="00039-1580">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="00039-1581">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="00039-1581">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="00039-1582">Cloud</span><span class="sxs-lookup"><span data-stu-id="00039-1582">Cloud</span></span>

* <span data-ttu-id="00039-1583">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="00039-1583">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="00039-1584">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1584">Container</span></span>

* <span data-ttu-id="00039-1585">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="00039-1585">Added support to open multiple ports</span></span>
* <span data-ttu-id="00039-1586">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="00039-1586">Added container group restart policy</span></span>
* <span data-ttu-id="00039-1587">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="00039-1587">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="00039-1588">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="00039-1588">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00039-1589">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00039-1589">Data Lake Analytics</span></span>

* <span data-ttu-id="00039-1590">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="00039-1590">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00039-1591">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-1591">Data Lake Store</span></span>

* <span data-ttu-id="00039-1592">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="00039-1592">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1593">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1593">Extension</span></span>

* <span data-ttu-id="00039-1594">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="00039-1594">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="00039-1595">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="00039-1595">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="00039-1596">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1596">IoT</span></span>

* <span data-ttu-id="00039-1597">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="00039-1597">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1598">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1598">Monitor</span></span>

* <span data-ttu-id="00039-1599">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="00039-1599">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="00039-1600">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1600">Network</span></span>

* <span data-ttu-id="00039-1601">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="00039-1601">Added support for CAA DNS records</span></span>
* <span data-ttu-id="00039-1602">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="00039-1602">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="00039-1603">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="00039-1603">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="00039-1604">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="00039-1604">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="00039-1605">Réservations</span><span class="sxs-lookup"><span data-stu-id="00039-1605">Reservations</span></span>

* <span data-ttu-id="00039-1606">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1606">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1607">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1607">Resource</span></span>

* <span data-ttu-id="00039-1608">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="00039-1608">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1609">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1609">SQL</span></span>

* <span data-ttu-id="00039-1610">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1610">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1611">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1611">Storage</span></span>

* <span data-ttu-id="00039-1612">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1612">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="00039-1613">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="00039-1613">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="00039-1614">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="00039-1614">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="00039-1615">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="00039-1615">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="00039-1616">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="00039-1616">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="00039-1617">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="00039-1617">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="00039-1618">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1618">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1619">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1619">VM</span></span>

* <span data-ttu-id="00039-1620">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="00039-1620">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="00039-1621">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="00039-1621">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="00039-1622">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="00039-1622">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="00039-1623">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="00039-1623">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="00039-1624">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="00039-1624">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="00039-1625">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1625">October 24, 2017</span></span>

<span data-ttu-id="00039-1626">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="00039-1626">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="00039-1627">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1627">Core</span></span>

* <span data-ttu-id="00039-1628">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="00039-1628">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1629">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1629">ACR</span></span>

* <span data-ttu-id="00039-1630">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="00039-1630">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="00039-1631">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="00039-1631">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="00039-1632">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="00039-1632">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1633">ACS</span></span>

* <span data-ttu-id="00039-1634">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="00039-1634">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="00039-1635">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="00039-1635">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1636">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1636">Appservice</span></span>

* <span data-ttu-id="00039-1637">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="00039-1637">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="00039-1638">Composant</span><span class="sxs-lookup"><span data-stu-id="00039-1638">Component</span></span>

* <span data-ttu-id="00039-1639">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="00039-1639">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1640">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1640">Monitor</span></span>

* <span data-ttu-id="00039-1641">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="00039-1641">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1642">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1642">Resource</span></span>

* <span data-ttu-id="00039-1643">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="00039-1643">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="00039-1644">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="00039-1644">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1645">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1645">VM</span></span>

* <span data-ttu-id="00039-1646">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00039-1646">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="00039-1647">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1647">October 9, 2017</span></span>

<span data-ttu-id="00039-1648">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="00039-1648">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="00039-1649">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1649">Core</span></span>

* <span data-ttu-id="00039-1650">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="00039-1650">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1651">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1651">Appservice</span></span>

* <span data-ttu-id="00039-1652">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="00039-1652">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="00039-1653">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1653">Batch</span></span>

* <span data-ttu-id="00039-1654">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="00039-1654">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="00039-1655">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="00039-1655">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="00039-1656">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1656">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="00039-1657">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="00039-1657">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="00039-1658">Batchai</span><span class="sxs-lookup"><span data-stu-id="00039-1658">Batchai</span></span>

* <span data-ttu-id="00039-1659">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="00039-1659">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-1660">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-1660">Keyvault</span></span>

* <span data-ttu-id="00039-1661">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="00039-1661">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="00039-1662">(#4448)</span><span class="sxs-lookup"><span data-stu-id="00039-1662">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="00039-1663">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1663">Network</span></span>

* <span data-ttu-id="00039-1664">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="00039-1664">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="00039-1665">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="00039-1665">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1666">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1666">Resource</span></span>

* <span data-ttu-id="00039-1667">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="00039-1667">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="00039-1668">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-1668">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="00039-1669">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="00039-1669">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="00039-1670">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="00039-1670">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1671">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1671">Sql</span></span>

* <span data-ttu-id="00039-1672">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="00039-1672">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="00039-1673">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="00039-1673">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="00039-1674">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="00039-1674">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1675">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1675">Storage</span></span>

* <span data-ttu-id="00039-1676">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="00039-1676">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1677">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1677">Vm</span></span>

* <span data-ttu-id="00039-1678">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="00039-1678">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="00039-1679">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00039-1679">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="00039-1680">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="00039-1680">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="00039-1681">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-1681">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="00039-1682">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00039-1682">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="00039-1683">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1683">September 22, 2017</span></span>

<span data-ttu-id="00039-1684">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="00039-1684">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1685">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1685">Resource</span></span>

* <span data-ttu-id="00039-1686">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="00039-1686">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="00039-1687">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="00039-1687">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="00039-1688">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="00039-1688">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="00039-1689">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="00039-1689">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="00039-1690">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1690">Network</span></span>

* <span data-ttu-id="00039-1691">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="00039-1691">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="00039-1692">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="00039-1692">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="00039-1693">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="00039-1693">Added `asg` application security group commands</span></span>
* <span data-ttu-id="00039-1694">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1694">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="00039-1695">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1695">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="00039-1696">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1696">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="00039-1697">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="00039-1697">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1698">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1698">Storage</span></span>

* <span data-ttu-id="00039-1699">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="00039-1699">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="00039-1700">Événement</span><span class="sxs-lookup"><span data-stu-id="00039-1700">Eventgrid</span></span>

* <span data-ttu-id="00039-1701">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="00039-1701">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1702">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1702">SQL</span></span>

* <span data-ttu-id="00039-1703">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="00039-1703">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="00039-1704">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="00039-1704">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="00039-1705">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1705">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-1706">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-1706">Keyvault</span></span>

* <span data-ttu-id="00039-1707">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="00039-1707">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1708">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1708">VM</span></span>

* <span data-ttu-id="00039-1709">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1709">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="00039-1710">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="00039-1710">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="00039-1711">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="00039-1711">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="00039-1712">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="00039-1712">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="00039-1713">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="00039-1713">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="00039-1714">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="00039-1714">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1715">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1715">ACS</span></span>

* <span data-ttu-id="00039-1716">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="00039-1716">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1717">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1717">Appservice</span></span>

* <span data-ttu-id="00039-1718">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="00039-1718">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="00039-1719">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="00039-1719">Backup</span></span>

* <span data-ttu-id="00039-1720">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="00039-1720">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="00039-1721">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1721">September 11, 2017</span></span>

<span data-ttu-id="00039-1722">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="00039-1722">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="00039-1723">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1723">Core</span></span>

* <span data-ttu-id="00039-1724">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="00039-1724">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="00039-1725">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="00039-1725">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1726">Acs</span><span class="sxs-lookup"><span data-stu-id="00039-1726">Acs</span></span>

* <span data-ttu-id="00039-1727">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="00039-1727">Added `acs list-locations` command</span></span>
* <span data-ttu-id="00039-1728">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="00039-1728">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1729">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1729">Appservice</span></span>

* <span data-ttu-id="00039-1730">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="00039-1730">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="00039-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="00039-1731">CDN</span></span>

* <span data-ttu-id="00039-1732">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="00039-1732">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="00039-1733">Extension</span><span class="sxs-lookup"><span data-stu-id="00039-1733">Extension</span></span>

* <span data-ttu-id="00039-1734">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1734">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-1735">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-1735">Keyvault</span></span>

* <span data-ttu-id="00039-1736">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="00039-1736">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="00039-1737">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1737">Network</span></span>

* <span data-ttu-id="00039-1738">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="00039-1738">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="00039-1739">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="00039-1739">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="00039-1740">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="00039-1740">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="00039-1741">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="00039-1741">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="00039-1742">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="00039-1742">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1743">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1743">Resource</span></span>

* <span data-ttu-id="00039-1744">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="00039-1744">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="00039-1745">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="00039-1745">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="00039-1746">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="00039-1746">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="00039-1747">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="00039-1747">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="00039-1748">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-1748">SQL</span></span>

* <span data-ttu-id="00039-1749">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="00039-1749">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1750">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1750">VM</span></span>

* <span data-ttu-id="00039-1751">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="00039-1751">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="00039-1752">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="00039-1752">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="00039-1753">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1753">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="00039-1754">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="00039-1754">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="00039-1755">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="00039-1755">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="00039-1756">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1756">August 31, 2017</span></span>

<span data-ttu-id="00039-1757">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="00039-1757">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-1758">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-1758">Keyvault</span></span>

* <span data-ttu-id="00039-1759">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="00039-1759">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="00039-1760">Sf</span><span class="sxs-lookup"><span data-stu-id="00039-1760">Sf</span></span>

* <span data-ttu-id="00039-1761">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="00039-1761">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1762">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1762">Storage</span></span>

* <span data-ttu-id="00039-1763">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="00039-1763">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="00039-1764">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="00039-1764">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="00039-1765">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1765">August 28, 2017</span></span>

<span data-ttu-id="00039-1766">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="00039-1766">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="00039-1767">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="00039-1767">CLI</span></span>

* <span data-ttu-id="00039-1768">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="00039-1768">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1769">ACS</span></span>

* <span data-ttu-id="00039-1770">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="00039-1770">Corrected preview regions</span></span>
* <span data-ttu-id="00039-1771">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="00039-1771">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="00039-1772">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1772">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1773">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1773">Appservice</span></span>

* <span data-ttu-id="00039-1774">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="00039-1774">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="00039-1775">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="00039-1775">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="00039-1776">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="00039-1776">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="00039-1777">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="00039-1777">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="00039-1778">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="00039-1778">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="00039-1779">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1779">IoT</span></span>

* <span data-ttu-id="00039-1780">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="00039-1780">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="00039-1781">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1781">Network</span></span>

* <span data-ttu-id="00039-1782">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="00039-1782">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="00039-1783">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1783">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="00039-1784">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00039-1784">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="00039-1785">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="00039-1785">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="00039-1786">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="00039-1786">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1787">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1787">Profile</span></span>

* <span data-ttu-id="00039-1788">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1788">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00039-1789">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00039-1789">Service Fabric</span></span>

* <span data-ttu-id="00039-1790">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="00039-1790">Preview release</span></span>
* <span data-ttu-id="00039-1791">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="00039-1791">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="00039-1792">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="00039-1792">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="00039-1793">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="00039-1793">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1794">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1794">Storage</span></span>

* <span data-ttu-id="00039-1795">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="00039-1795">Enabled setting blob tier</span></span>
* <span data-ttu-id="00039-1796">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="00039-1796">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="00039-1797">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="00039-1797">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="00039-1798">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="00039-1798">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="00039-1799">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="00039-1799">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="00039-1800">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="00039-1800">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1801">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1801">VM</span></span>

* <span data-ttu-id="00039-1802">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="00039-1802">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="00039-1803">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="00039-1803">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="00039-1804">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00039-1804">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="00039-1805">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="00039-1805">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="00039-1806">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="00039-1806">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="00039-1807">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="00039-1807">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="00039-1808">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1808">August 15, 2017</span></span>

<span data-ttu-id="00039-1809">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="00039-1809">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1810">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1810">ACS</span></span>

* <span data-ttu-id="00039-1811">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="00039-1811">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1812">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1812">Appservice</span></span>

* <span data-ttu-id="00039-1813">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="00039-1813">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="00039-1814">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00039-1814">Event Grid</span></span>

* <span data-ttu-id="00039-1815">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="00039-1815">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="00039-1816">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1816">August 11, 2017</span></span>

<span data-ttu-id="00039-1817">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="00039-1817">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1818">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1818">ACS</span></span>

* <span data-ttu-id="00039-1819">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="00039-1819">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="00039-1820">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1820">Batch</span></span>

* <span data-ttu-id="00039-1821">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="00039-1821">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="00039-1822">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="00039-1822">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="00039-1823">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="00039-1823">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="00039-1824">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="00039-1824">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="00039-1825">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="00039-1825">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="00039-1826">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="00039-1826">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="00039-1827">Composant</span><span class="sxs-lookup"><span data-stu-id="00039-1827">Component</span></span>

* <span data-ttu-id="00039-1828">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="00039-1828">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="00039-1829">Conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1829">Container</span></span>

* <span data-ttu-id="00039-1830">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="00039-1830">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="00039-1831">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-1831">Data Lake Store</span></span>

* <span data-ttu-id="00039-1832">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="00039-1832">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="00039-1833">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00039-1833">Event Grid</span></span>

* <span data-ttu-id="00039-1834">Version initiale</span><span class="sxs-lookup"><span data-stu-id="00039-1834">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="00039-1835">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1835">Network</span></span>

* <span data-ttu-id="00039-1836">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="00039-1836">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="00039-1837">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="00039-1837">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="00039-1838">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="00039-1838">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="00039-1839">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="00039-1839">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1840">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1840">Profile</span></span>

* <span data-ttu-id="00039-1841">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="00039-1841">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="00039-1842">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-1842">Storage</span></span>

* <span data-ttu-id="00039-1843">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="00039-1843">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="00039-1844">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-1844">VM</span></span>

* <span data-ttu-id="00039-1845">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="00039-1845">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="00039-1846">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="00039-1846">Exposed `list-skus` command</span></span>
* <span data-ttu-id="00039-1847">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="00039-1847">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="00039-1848">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="00039-1848">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="00039-1849">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="00039-1849">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="00039-1850">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="00039-1850">July 28, 2017</span></span>

<span data-ttu-id="00039-1851">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="00039-1851">Version 2.0.12</span></span>

* <span data-ttu-id="00039-1852">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="00039-1852">Added container commands</span></span>
* <span data-ttu-id="00039-1853">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="00039-1853">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="00039-1854">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-1854">Core</span></span>

* <span data-ttu-id="00039-1855">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="00039-1855">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="00039-1856">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="00039-1856">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="00039-1857">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="00039-1857">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="00039-1858">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="00039-1858">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="00039-1859">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="00039-1859">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="00039-1860">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="00039-1860">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="00039-1861">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="00039-1861">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="00039-1862">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="00039-1862">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="00039-1863">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="00039-1863">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="00039-1864">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="00039-1864">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="00039-1865">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="00039-1865">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="00039-1866">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="00039-1866">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="00039-1867">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="00039-1867">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="00039-1868">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="00039-1868">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="00039-1869">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="00039-1869">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="00039-1870">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="00039-1870">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="00039-1871">ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1871">ACR</span></span>

* <span data-ttu-id="00039-1872">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="00039-1872">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="00039-1873">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="00039-1873">Support SKU update for managed registries</span></span>
* <span data-ttu-id="00039-1874">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="00039-1874">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="00039-1875">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="00039-1875">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="00039-1876">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="00039-1876">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="00039-1877">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="00039-1877">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="00039-1878">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-1878">ACS</span></span>

* <span data-ttu-id="00039-1879">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="00039-1879">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-1880">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-1880">Appservice</span></span>

* <span data-ttu-id="00039-1881">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="00039-1881">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="00039-1882">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="00039-1882">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="00039-1883">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="00039-1883">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="00039-1884">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="00039-1884">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="00039-1885">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="00039-1885">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="00039-1886">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="00039-1886">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="00039-1887">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="00039-1887">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="00039-1888">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="00039-1888">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="00039-1889">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="00039-1889">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="00039-1890">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="00039-1890">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="00039-1891">Batch</span><span class="sxs-lookup"><span data-stu-id="00039-1891">Batch</span></span>

* <span data-ttu-id="00039-1892">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="00039-1892">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="00039-1893">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="00039-1893">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="00039-1894">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="00039-1894">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="00039-1895">CDN</span><span class="sxs-lookup"><span data-stu-id="00039-1895">CDN</span></span>

* <span data-ttu-id="00039-1896">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="00039-1896">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="00039-1897">Cloud</span><span class="sxs-lookup"><span data-stu-id="00039-1897">Cloud</span></span>

* <span data-ttu-id="00039-1898">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="00039-1898">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="00039-1899">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="00039-1899">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="00039-1900">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="00039-1900">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="00039-1901">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="00039-1901">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="00039-1902">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="00039-1902">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-1903">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-1903">CosmosDB</span></span>

* <span data-ttu-id="00039-1904">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="00039-1904">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="00039-1905">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="00039-1905">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00039-1906">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00039-1906">Data Lake Analytics</span></span>

* <span data-ttu-id="00039-1907">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="00039-1907">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="00039-1908">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="00039-1908">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="00039-1909">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="00039-1909">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00039-1910">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-1910">Data Lake Store</span></span>

* <span data-ttu-id="00039-1911">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="00039-1911">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="00039-1912">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="00039-1912">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="00039-1913">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="00039-1913">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="00039-1914">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-1914">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="00039-1915">Interactive</span><span class="sxs-lookup"><span data-stu-id="00039-1915">Interactive</span></span>

* <span data-ttu-id="00039-1916">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="00039-1916">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="00039-1917">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="00039-1917">Increased test coverage</span></span>
* <span data-ttu-id="00039-1918">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="00039-1918">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="00039-1919">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="00039-1919">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="00039-1920">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="00039-1920">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="00039-1921">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="00039-1921">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="00039-1922">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="00039-1922">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="00039-1923">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="00039-1923">Added `--progress` flag</span></span>
* <span data-ttu-id="00039-1924">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="00039-1924">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="00039-1925">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="00039-1925">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="00039-1926">IoT</span><span class="sxs-lookup"><span data-stu-id="00039-1926">IoT</span></span>

* <span data-ttu-id="00039-1927">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="00039-1927">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="00039-1928">(#3934)</span><span class="sxs-lookup"><span data-stu-id="00039-1928">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="00039-1929">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="00039-1929">Key vault</span></span>

* <span data-ttu-id="00039-1930">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="00039-1930">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="00039-1931">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00039-1931">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="00039-1932">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00039-1932">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="00039-1933">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00039-1933">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="00039-1934">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00039-1934">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="00039-1935">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="00039-1935">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="00039-1936">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="00039-1936">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="00039-1937">(#3307)</span><span class="sxs-lookup"><span data-stu-id="00039-1937">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="00039-1938">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-1938">Lab</span></span>

* <span data-ttu-id="00039-1939">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="00039-1939">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="00039-1940">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="00039-1940">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-1941">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-1941">Monitor</span></span>

* <span data-ttu-id="00039-1942">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="00039-1942">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="00039-1943">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="00039-1943">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="00039-1944">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="00039-1944">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="00039-1945">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="00039-1945">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="00039-1946">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="00039-1946">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="00039-1947">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="00039-1947">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="00039-1948">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="00039-1948">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="00039-1949">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="00039-1949">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="00039-1950">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="00039-1950">`location` no longer required</span></span>
  * <span data-ttu-id="00039-1951">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="00039-1951">Add name and ID support for target</span></span>
  * <span data-ttu-id="00039-1952">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="00039-1952">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="00039-1953">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="00039-1953">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="00039-1954">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="00039-1954">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="00039-1955">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="00039-1955">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="00039-1956">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="00039-1956">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="00039-1957">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="00039-1957">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="00039-1958">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-1958">Network</span></span>

* <span data-ttu-id="00039-1959">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="00039-1959">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="00039-1960">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="00039-1960">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="00039-1961">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="00039-1961">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="00039-1962">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="00039-1962">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="00039-1963">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="00039-1963">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="00039-1964">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="00039-1964">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="00039-1965">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="00039-1965">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="00039-1966">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="00039-1966">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="00039-1967">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="00039-1967">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="00039-1968">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="00039-1968">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="00039-1969">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="00039-1969">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="00039-1970">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="00039-1970">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="00039-1971">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="00039-1971">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="00039-1972">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="00039-1972">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="00039-1973">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="00039-1973">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="00039-1974">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="00039-1974">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="00039-1975">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="00039-1975">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="00039-1976">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="00039-1976">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="00039-1977">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="00039-1977">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="00039-1978">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="00039-1978">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="00039-1979">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="00039-1979">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="00039-1980">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-1980">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="00039-1981">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="00039-1981">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="00039-1982">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="00039-1982">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="00039-1983">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="00039-1983">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="00039-1984">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="00039-1984">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="00039-1985">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="00039-1985">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="00039-1986">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-1986">Profile</span></span>

* <span data-ttu-id="00039-1987">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="00039-1987">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="00039-1988">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="00039-1988">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="00039-1989">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="00039-1989">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="00039-1990">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="00039-1990">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="00039-1991">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="00039-1991">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="00039-1992">SGBDR</span><span class="sxs-lookup"><span data-stu-id="00039-1992">RDBMS</span></span>

* <span data-ttu-id="00039-1993">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="00039-1993">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="00039-1994">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="00039-1994">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="00039-1995">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="00039-1995">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="00039-1996">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="00039-1996">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="00039-1997">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-1997">Resource</span></span>

* <span data-ttu-id="00039-1998">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="00039-1998">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="00039-1999">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="00039-1999">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="00039-2000">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="00039-2000">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="00039-2001">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="00039-2001">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="00039-2002">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="00039-2002">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="00039-2003">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="00039-2003">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="00039-2004">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="00039-2004">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="00039-2005">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="00039-2005">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="00039-2006">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-2006">Role</span></span>

* <span data-ttu-id="00039-2007">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="00039-2007">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="00039-2008">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="00039-2008">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="00039-2009">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="00039-2009">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="00039-2010">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="00039-2010">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="00039-2011">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="00039-2011">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00039-2012">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00039-2012">Service Fabric</span></span>
* <span data-ttu-id="00039-2013">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="00039-2013">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="00039-2014">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="00039-2014">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="00039-2015">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="00039-2015">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="00039-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-2016">SQL</span></span>

* <span data-ttu-id="00039-2017">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="00039-2017">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="00039-2018">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="00039-2018">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="00039-2019">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="00039-2019">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="00039-2020">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-2020">Storage</span></span>

* <span data-ttu-id="00039-2021">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="00039-2021">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="00039-2022">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="00039-2022">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="00039-2023">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="00039-2023">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="00039-2024">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="00039-2024">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="00039-2025">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="00039-2025">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="00039-2026">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="00039-2026">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="00039-2027">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-2027">VM</span></span>

* <span data-ttu-id="00039-2028">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="00039-2028">Support configuring nsg</span></span>
* <span data-ttu-id="00039-2029">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="00039-2029">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="00039-2030">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="00039-2030">Support managed service identities</span></span>
* <span data-ttu-id="00039-2031">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="00039-2031">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="00039-2032">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="00039-2032">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="00039-2033">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="00039-2033">May 10, 2017</span></span>

<span data-ttu-id="00039-2034">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="00039-2034">Version 2.0.6</span></span>

* <span data-ttu-id="00039-2035">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="00039-2035">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="00039-2036">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="00039-2036">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="00039-2037">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-2037">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="00039-2038">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00039-2038">Include Cognitive Services module</span></span>
* <span data-ttu-id="00039-2039">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00039-2039">Include Service Fabric module</span></span>
* <span data-ttu-id="00039-2040">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="00039-2040">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="00039-2041">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="00039-2041">Add support for CDN commands</span></span>
* <span data-ttu-id="00039-2042">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="00039-2042">Remove Container module</span></span>
* <span data-ttu-id="00039-2043">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="00039-2043">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="00039-2044">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="00039-2044">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="00039-2045">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-2045">Core</span></span>

* <span data-ttu-id="00039-2046">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="00039-2046">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="00039-2047">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="00039-2047">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="00039-2048">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="00039-2048">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="00039-2049">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="00039-2049">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="00039-2050">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="00039-2050">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="00039-2051">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="00039-2051">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="00039-2052">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="00039-2052">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="00039-2053">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="00039-2053">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="00039-2054">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="00039-2054">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="00039-2055">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="00039-2055">core: Improved performance</span></span>
* <span data-ttu-id="00039-2056">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="00039-2056">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="00039-2057">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="00039-2057">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="00039-2058">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-2058">ACS</span></span>

* <span data-ttu-id="00039-2059">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="00039-2059">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="00039-2060">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="00039-2060">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="00039-2061">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="00039-2061">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="00039-2062">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="00039-2062">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-2063">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-2063">AppService</span></span>

* <span data-ttu-id="00039-2064">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="00039-2064">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="00039-2065">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="00039-2065">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="00039-2066">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="00039-2066">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="00039-2067">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="00039-2067">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="00039-2068">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="00039-2068">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="00039-2069">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="00039-2069">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="00039-2070">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="00039-2070">support slot swap with preview</span></span>
* <span data-ttu-id="00039-2071">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="00039-2071">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="00039-2072">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="00039-2072">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00039-2073">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00039-2073">CosmosDB</span></span>

* <span data-ttu-id="00039-2074">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="00039-2074">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="00039-2075">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="00039-2075">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="00039-2076">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="00039-2076">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="00039-2077">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="00039-2077">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00039-2078">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00039-2078">Data Lake Analytics</span></span>

* <span data-ttu-id="00039-2079">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="00039-2079">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="00039-2080">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="00039-2080">Add support for new catalog item type: package.</span></span> <span data-ttu-id="00039-2081">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="00039-2081">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="00039-2082">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="00039-2082">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="00039-2083">Table</span><span class="sxs-lookup"><span data-stu-id="00039-2083">Table</span></span>
  * <span data-ttu-id="00039-2084">Fonction table</span><span class="sxs-lookup"><span data-stu-id="00039-2084">Table valued function</span></span>
  * <span data-ttu-id="00039-2085">Affichage</span><span class="sxs-lookup"><span data-stu-id="00039-2085">View</span></span>
  * <span data-ttu-id="00039-2086">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="00039-2086">Table Statistics.</span></span> <span data-ttu-id="00039-2087">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="00039-2087">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00039-2088">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-2088">Data Lake Store</span></span>

* <span data-ttu-id="00039-2089">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="00039-2089">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="00039-2090">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="00039-2090">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="00039-2091">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="00039-2091">missed help for access show.</span></span> <span data-ttu-id="00039-2092">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="00039-2092">adding it.</span></span> <span data-ttu-id="00039-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="00039-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="00039-2094">Rechercher</span><span class="sxs-lookup"><span data-stu-id="00039-2094">Find</span></span>

* <span data-ttu-id="00039-2095">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="00039-2095">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="00039-2096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00039-2096">KeyVault</span></span>

* <span data-ttu-id="00039-2097">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="00039-2097">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="00039-2098">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="00039-2098">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="00039-2099">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="00039-2099">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="00039-2100">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="00039-2100">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="00039-2101">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="00039-2101">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="00039-2102">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2102">Lab</span></span>

* <span data-ttu-id="00039-2103">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2103">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="00039-2104">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2104">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="00039-2105">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2105">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="00039-2106">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2106">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="00039-2107">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="00039-2107">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="00039-2108">Surveiller</span><span class="sxs-lookup"><span data-stu-id="00039-2108">Monitor</span></span>

* <span data-ttu-id="00039-2109">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="00039-2109">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="00039-2110">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="00039-2110">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="00039-2111">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-2111">Network</span></span>

* <span data-ttu-id="00039-2112">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="00039-2112">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="00039-2113">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="00039-2113">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="00039-2114">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="00039-2114">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="00039-2115">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="00039-2115">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="00039-2116">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="00039-2116">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="00039-2117">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="00039-2117">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="00039-2118">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="00039-2118">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="00039-2119">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="00039-2119">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="00039-2120">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="00039-2120">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="00039-2121">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="00039-2121">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="00039-2122">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="00039-2122">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="00039-2123">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="00039-2123">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="00039-2124">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="00039-2124">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="00039-2125">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="00039-2125">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="00039-2126">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="00039-2126">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="00039-2127">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="00039-2127">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="00039-2128">Profil</span><span class="sxs-lookup"><span data-stu-id="00039-2128">Profile</span></span>

* <span data-ttu-id="00039-2129">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="00039-2129">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="00039-2130">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="00039-2130">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="00039-2131">Redis</span><span class="sxs-lookup"><span data-stu-id="00039-2131">Redis</span></span>

* <span data-ttu-id="00039-2132">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="00039-2132">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="00039-2133">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="00039-2133">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="00039-2134">Ressource</span><span class="sxs-lookup"><span data-stu-id="00039-2134">Resource</span></span>

* <span data-ttu-id="00039-2135">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="00039-2135">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="00039-2136">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="00039-2136">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="00039-2137">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="00039-2137">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="00039-2138">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="00039-2138">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="00039-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="00039-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="00039-2140">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="00039-2140">Add docs for az lock update.</span></span> <span data-ttu-id="00039-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="00039-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="00039-2142">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="00039-2142">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="00039-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="00039-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="00039-2144">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="00039-2144">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="00039-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="00039-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="00039-2146">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="00039-2146">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="00039-2147">Rôle</span><span class="sxs-lookup"><span data-stu-id="00039-2147">Role</span></span>

* <span data-ttu-id="00039-2148">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="00039-2148">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="00039-2149">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="00039-2149">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="00039-2150">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="00039-2150">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="00039-2151">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="00039-2151">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="00039-2152">SQL</span><span class="sxs-lookup"><span data-stu-id="00039-2152">SQL</span></span>

* <span data-ttu-id="00039-2153">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="00039-2153">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="00039-2154">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="00039-2154">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="00039-2155">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-2155">Storage</span></span>

* <span data-ttu-id="00039-2156">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="00039-2156">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="00039-2157">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="00039-2157">Add support for incremental blob copy</span></span>
* <span data-ttu-id="00039-2158">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="00039-2158">Add support for large block blob upload</span></span>
* <span data-ttu-id="00039-2159">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="00039-2159">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="00039-2160">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-2160">VM</span></span>

* <span data-ttu-id="00039-2161">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="00039-2161">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="00039-2162">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="00039-2162">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="00039-2163">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="00039-2163">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="00039-2164">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="00039-2164">az vm/vmss disk</span></span>
  3. <span data-ttu-id="00039-2165">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="00039-2165">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="00039-2166">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="00039-2166">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="00039-2167">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="00039-2167">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="00039-2168">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="00039-2168">April 3, 2017</span></span>

<span data-ttu-id="00039-2169">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="00039-2169">Version 2.0.2</span></span>

<span data-ttu-id="00039-2170">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="00039-2170">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="00039-2171">Principal</span><span class="sxs-lookup"><span data-stu-id="00039-2171">Core</span></span>

* <span data-ttu-id="00039-2172">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-2172">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="00039-2173">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="00039-2173">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="00039-2174">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="00039-2174">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="00039-2175">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="00039-2175">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="00039-2176">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="00039-2176">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="00039-2177">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="00039-2177">Add prompting for missing template parameters.</span></span> <span data-ttu-id="00039-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="00039-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="00039-2179">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="00039-2179">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="00039-2180">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="00039-2180">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="00039-2181">ACS</span><span class="sxs-lookup"><span data-stu-id="00039-2181">ACS</span></span>

* <span data-ttu-id="00039-2182">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="00039-2182">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="00039-2183">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="00039-2183">Add support for ssh key password prompting.</span></span> <span data-ttu-id="00039-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="00039-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="00039-2185">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="00039-2185">Add support for windows clusters.</span></span> <span data-ttu-id="00039-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="00039-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="00039-2187">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="00039-2187">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="00039-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="00039-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="00039-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="00039-2189">AppService</span></span>

* <span data-ttu-id="00039-2190">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="00039-2190">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="00039-2191">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="00039-2191">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="00039-2192">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="00039-2192">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="00039-2193">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="00039-2193">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="00039-2194">DataLake</span><span class="sxs-lookup"><span data-stu-id="00039-2194">DataLake</span></span>

* <span data-ttu-id="00039-2195">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00039-2195">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="00039-2196">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00039-2196">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="00039-2197">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="00039-2197">DocuemntDB</span></span>

* <span data-ttu-id="00039-2198">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="00039-2198">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="00039-2199">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="00039-2199">VM</span></span>

* <span data-ttu-id="00039-2200">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="00039-2200">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="00039-2201">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="00039-2201">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="00039-2202">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="00039-2202">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="00039-2203">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="00039-2203">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="00039-2204">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="00039-2204">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="00039-2205">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="00039-2205">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="00039-2206">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="00039-2206">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="00039-2207">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="00039-2207">February 27, 2017</span></span>

<span data-ttu-id="00039-2208">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="00039-2208">Version 2.0.0</span></span>

<span data-ttu-id="00039-2209">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="00039-2209">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="00039-2210">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="00039-2210">Container Service (acs)</span></span>
- <span data-ttu-id="00039-2211">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="00039-2211">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="00039-2212">Réseau</span><span class="sxs-lookup"><span data-stu-id="00039-2212">Networking</span></span>
- <span data-ttu-id="00039-2213">Stockage</span><span class="sxs-lookup"><span data-stu-id="00039-2213">Storage</span></span>

<span data-ttu-id="00039-2214">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="00039-2214">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="00039-2215">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00039-2215">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="00039-2216">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="00039-2216">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="00039-2217">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="00039-2217">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="00039-2218">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="00039-2218">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="00039-2219">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="00039-2219">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="00039-2220">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="00039-2220">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="00039-2221">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="00039-2221">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="00039-2222">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="00039-2222">Provide feedback from the command line with the `az feedback` command</span></span>

